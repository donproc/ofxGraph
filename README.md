ofxGraph
====

## Description
ofxGraph is a graph plotting addon for openframeworks.

1. single/multiple plot
2. Manual adjustable graph size and position
3. detailed plot data information
4. Adjustable buffer size
5. CSV file export with a save dialog
6. Automatic saving(position and size). except for ofxGui settings.

## Usage
```c++
void ofApp::setup(){

// ofxGraph Init
  graph.setup("sample");
  graph.setDx(1.0); // which means delta of time
  graph.setColor(ofColor::white);  // ofColor(255,255,255)
}
void ofApp::update(){
  // plot a random data on a each frame
  graph.add(ofRandom(-100,100));
}

void ofApp::draw(){
  ofBackground(50,50,50);
  graph.draw();
}
```
See Example for more detailed.

![Example screenshot](/screenshot.png)

## Install
ofxGui and ofxXmlSettings are required.

## Licence
[MIT](https://opensource.org/licenses/MIT)

## Author
[TetsuakiBaba](https://github.com/TetsuakiBaba)
