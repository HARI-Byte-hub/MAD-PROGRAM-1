import 'package:flutter/material.dart';
void main() => runApp(MaterialApp(
      home: MyDetails(),
      debugShowCheckedModeBanner: false,
    ));
class MyDetails extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Personal Details'),
        backgroundColor: Colors.blueAccent,
      ),
      backgroundColor: Colors.grey[200],
      body: Center(
        child: Container(
          padding: EdgeInsets.all(20),
          width: 300,
          decoration: BoxDecoration(
            color: Colors.white,
            borderRadius: BorderRadius.circular(12),
            boxShadow: [
            
                  
                BoxShadow(blurRadius: 5, color: Colors.grey),
            ],
          ),
          child: Column(
            mainAxisSize: MainAxisSize.min,
            crossAxisAlignment: CrossAxisAlignment.start,
            children: [
            Text('Name: Alex Smith', style: TextStyle(fontSize: 18)),
              SizedBox(height: 10),
              Text('Age: 22', style: TextStyle(fontSize: 18)),
              SizedBox(height: 10),
              Text('Email: alex.smith@example.com', style: TextStyle(fontSize: 18)),
              SizedBox(height: 10),
              Text('City: Los Angeles', style: TextStyle(fontSize: 18)),
            ],
          ),
        ),
      ),
    );
  }
}
