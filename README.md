import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          backgroundColor: Colors.blue,
          title: const Text(
            'sample App',
            style: TextStyle(color: Colors.white),
          ),
        ),
        body: Center(
          child: Padding(
            padding: const EdgeInsets.only(
              left: 25,
              right: 25,
            ),
            child: Column(
              children: [
                const Text(
                  'TutorialKart',
                  style: TextStyle(
                    color: Colors.blue,
                    fontSize: 40.0,
                  ),
                ),
                const Text(
                  'Sign In',
                  style: TextStyle(
                    color: Colors.red,
                    fontSize: 20.0,
                  ),
                ),
                const SizedBox(
                  height: 15,
                ),
                TextFormField(
                  decoration: const InputDecoration(
                    hintStyle: TextStyle(color: Colors.grey),
                    hintText: 'User Name',
                    border: OutlineInputBorder(),
                  ),
                ),
                const SizedBox(
                  height: 18,
                ),
                TextFormField(
                  decoration: const InputDecoration(
                    hintStyle: TextStyle(color: Colors.grey),
                    hintText: 'Password',
                    border: OutlineInputBorder(),
                  ),
                ),
                const SizedBox(
                  height: 18,
                ),
                const Text(
                  'Forget Password',
                  style: TextStyle(
                    color: Colors.blue,
                    fontSize: 18.0,
                  ),
                ),
                ElevatedButton(
                  onPressed: () {},
                  child: const Text('Login'),
                ),
                const Center(
                  child: Center(
                    child: Row(
                      mainAxisAlignment: MainAxisAlignment.center,
                      children: [
                        Text('Dose not have account ?'),
                        Text(
                          'Signin',
                          style: TextStyle(color: Colors.blue),
                        )
                      ],
                    ),
                  ),
                ),
              ],
            ),
          ),
        ),
      ),
    );
  }
}
