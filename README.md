# flutter-dart-notes
 Flutter/Dart öğrenirken alacağım tüm notlar için bir repo
 ## freeCodeCamp video(37 saat)
 #### Future
  ```dart
Future<int> multipliesByTwo(int a){
	return Future.delayed(const Duration(seconds: 3), () {
		return a*2;
	});
}

void test async {
	final result = await multipliesByTwo(100);
	print(result);
}
```
#### Stream
A pipe of `Future`
 ```dart
Stream<string> getName{
	return Stream.periodic(const Duration(seconds: 1), () {
		return 'Foo';
	});
}

void test async{
	await for (final value in getName()){
		print(value);
	}
	print("Stream finished working.") //Never prints
}
```
### Other
 - pubspec.yaml: It holds critical data about application.
 - >flutter pub add dependency_name

## Docs

 -Widgets

