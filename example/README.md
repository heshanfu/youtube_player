# youtube_player_example


```dart
class _MyHomePageState extends State<MyHomePage> {
  TextEditingController _idController = TextEditingController();
  String id = "nPt8bK2gbaU";

  @override
  Widget build(BuildContext context) {
    return Scaffold(
        appBar: AppBar(
          title: Text(widget.title),
        ),
        body: SingleChildScrollView(
          child: Column(
            mainAxisAlignment: MainAxisAlignment.start,
            children: <Widget>[
              YoutubePlayer(
                source: id,
                quality: YoutubeQuality.HD,
              ),
              Padding(
                padding: const EdgeInsets.all(8.0),
                child: TextFormField(
                  controller: _idController,
                  decoration: InputDecoration(
                    border: OutlineInputBorder(),
                    hintText: "Enter youtube \<video id\> or \<link\>"
                  ),
                ),
              ),
              RaisedButton(
                onPressed: () {
                  setState(() {
                    id = _idController.text;
                  });
                },
                child: Text("Play"),
              ),
            ],
          ),
        ));
  }
}
```