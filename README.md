## 1주차
안드로이드 스튜디오로 플러터 개발 환경 구성 및 최초 HelloWorld 앱 실행
![화면 캡처 2025-03-15 233422](https://github.com/user-attachments/assets/7a55a265-f7ba-4800-ab46-db222ecec443)

* C드라이브에 sdk압출풀어서 안드로이드스튜디오로 플러터 실행시키면 데몬오류뜸. 플러터닥터도 오류남 고로 내 문서에 압축풀어서 실행시킬것.
* 관련자료 https://github.com/flutter/flutter/issues/87383#issuecomment-948081570
* 에 해당하는 해결댓글
I had the same issue when I installed flutter on my f: drive (e.g. f:\flutter). The Flutter Windows installation instructions does not say "you must install flutter in C:\Users<your-user-name>\Documents," but, it turns out that the Flutter plugin expects that one has done so. The error message about increasing the number of file handles led me astray and wasted my time. After looking into increasing the number of file handles and getting lost, I checked the Flutter plugins default Flutter SDK path and saw it was wrong. Once fixed all is well.
I think either there should be no default Flutter SDK path or the installation documentation should have a note that says if Flutter is not installed in C:\Users<your-user-name>\Documents be sure to adjust the Flutter plugin settings.
