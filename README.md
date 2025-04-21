import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: ListViewDemo(),
 );
 }
}
class ListViewDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('ListView Example')),
 body: ListView(
 children: <Widget>[
 ListTile(
 leading: Icon(Icons.home),
 title: Text('Home'),
 onTap: () {
 print('Home tapped!');
 },
 ),
 ListTile(
 leading: Icon(Icons.person),
 title: Text('Profile'),
 onTap: () {
 print('Profile tapped!');
 },
 ),
 ListTile(
 leading: Icon(Icons.settings),
 title: Text('Settings'),
 onTap: () {
 print('Settings tapped!');
 },
 ),
 ListTile(
 leading: Icon(Icons.info),
 title: Text('About'),
 onTap: () {
 print('About tapped!');
 },
 ),
 ],
 ),
 );
 }
}
