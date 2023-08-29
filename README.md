//TextField widget
import 'package:flutter/material.dart';

void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("text widget"),
        ),
        body: Material(
          child: Center(
            child: Container(
              margin: EdgeInsets.all(22),
              child: TextField(
                undoController: UndoHistoryController(),
                maxLength: 39,
                textCapitalization: TextCapitalization.characters,
                textAlign: TextAlign.center,
                keyboardType: TextInputType.emailAddress,
                decoration: InputDecoration(
                  hintText: "Enter Your Name",
                  label: Text("Name"),
                  icon: Icon(Icons.person),
                  prefixIcon: Icon(Icons.access_alarm_outlined),
                  suffixIcon: Icon(Icons.ac_unit),
                  border: OutlineInputBorder(),
                  hintStyle: TextStyle(fontSize: 21, color: Colors.green),
                  labelStyle: TextStyle(color: Colors.red),
                ),
              ),
            ),
          ),
        ),
      ),
    ),
  );
}
