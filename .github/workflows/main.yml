dart

import 'package:flutter/material.dart';


void main() {

  runApp(const AlLisanApp());

}


class AlLisanApp extends StatelessWidget {

  const AlLisanApp({super.key});


  @override

  Widget build(BuildContext context) {

    return MaterialApp(

      debugShowCheckedModeBanner: false,

      title: 'اللسان المسلم',

      theme: ThemeData(

        colorScheme: ColorScheme.fromSeed(

          seedColor: const Color(0xFF176B50),

        ),

        useMaterial3: true,

        fontFamily: 'Arial',

      ),

      home: const HomePage(),

    );

  }

}


class HomePage extends StatelessWidget {

  const HomePage({super.key});


  final List<Map<String, String>> languages = const [

    {'name': 'الإنجليزية الأمريكية', 'flag': '🇺🇸'},

    {'name': 'الفرنسية', 'flag': '🇫🇷'},

    {'name': 'الألمانية', 'flag': '🇩🇪'},

    {'name': 'الإسبانية', 'flag': '🇪🇸'},

    {'name': 'التركية', 'flag': '🇹🇷'},

    {'name': 'الإيطالية', 'flag': '🇮🇹'},

  ];


  @override

  Widget build(BuildContext context) {

    return Directionality(

      textDirection: TextDirection.rtl,

      child: Scaffold(

        backgroundColor: const Color(0xFFF5F8F5),

        appBar: AppBar(

          backgroundColor: const Color(0xFF176B50),

          foregroundColor: Colors.white,

          title: const Text(

            'اللسان المسلم',

            style: TextStyle(fontWeight: FontWeight.bold),

          ),

          centerTitle: true,

        ),

        body: ListView(

          padding: const EdgeInsets.all(18),

          children: [

            const SizedBox(height: 15),

            const Icon(

              Icons.menu_book_rounded,

              size: 75,

              color: Color(0xFF176B50),

            ),

            const SizedBox(height: 12),

            const Text(

              'تعلّم لغة جديدة كل يوم',

              textAlign: TextAlign.center,

              style: TextStyle(

                fontSize: 24,

                fontWeight: FontWeight.bold,

                color: Color(0xFF176B50),

              ),

            ),

            const SizedBox(height: 8),

            const Text(

              'تعليم هادف ومفيد، في بيئة تراعي الضوابط الإسلامية.',

              textAlign: TextAlign.center,

              style: TextStyle(fontSize: 15),

            ),

            const SizedBox(height: 28),

            const Text(

              'اختر اللغة التي تريد تعلمها:',

              style: TextStyle(

                fontSize: 19,

                fontWeight: FontWeight.bold,

              ),

            ),

            const SizedBox(height: 12),

            ...languages.map(

              (language) => Card(

                margin: const EdgeInsets.only(bottom: 10),

                child: ListTile(

                  leading: Text(

                    language['flag']!,

                    style: const TextStyle(fontSize: 30),

                  ),

                  title: Text(

                    language['name']!,

                    style: const TextStyle(

                      fontWeight: FontWeight.bold,

                      fontSize: 17,

                    ),

                  ),

                  trailing: const Icon(

                    Icons.arrow_back_ios_new,

                    color: Color(0xFF176B50),

                  ),

                  onTap: () {

                    ScaffoldMessenger.of(context).showSnackBar(

                      SnackBar(

                        content: Text(

                          'سيتم إعداد دروس ${language['name']} قريبًا.',

                        ),

                      ),

                    );

                  },

                ),

              ),

            ),

            const SizedBox(height: 20),

            const Text(

              'نسأل الله أن يجعل هذا العلم نافعًا.',

              textAlign: TextAlign.center,

              style: TextStyle(

                color: Color(0xFF176B50),

                fontSize: 14,

              ),

            ),

          ],

        ),

      ),

    );

  }

}

