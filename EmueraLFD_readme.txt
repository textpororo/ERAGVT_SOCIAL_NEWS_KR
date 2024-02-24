Name : EmueraLFD
Version : V8
Deveoper : 굴러가는곰 (RollingBear)
Latest Update : 2023-03-21
Original Application:Emuera1.824 (Developed by 妊）|дﾟ)の中の人 and MinorShift), EmueraEE from Enter, ezEmuera from Riey

[라이센스 관련]
- 본 프로그램은 ezEmuera, EmueraEE, WebP 통합 지원 및 로딩 속도 개선을 위해 만들었습니다.
- EE 관련 기능은 EmueraEE by Enter, ezEmuera 쪽은 ezEmuera by Riey 쪽의 기능을 가져왔습니다.
- WebP, Sqlite를 제외한 대부분의 기능이 역설계를 통해 이뤄졌습니다.
- 각 기능은 각 기능을 개발한 개발자에게 권한이 있으며, 기본 앱은 Emuera 개발자에게 권한이 있습니다.
- 기본 라이센스는 Emuera_readme.txt 에 적혀 있으며 EmueraLFD는 별도의 라이센스나 권리가 없습니다.
- 기본 Emuera 기능을 고친거라 妊）|дﾟ)の中の人, MinorShift, Enter, Riey 에게 연락하시면 안됩니다.

[요약]
- WebP 지원
- 이미지를 모두 로드하지 않으며, resources 디렉토리에서 직접 읽어옴
- 옵션값 イメージチェック無視 를 통해 이미지 체크 과정을 모두 건너뛸 수 있음 (로딩 속도 향상)
    YES : 건너뜀, NO : 이미지 체크함

- Sqlite 지원
- 첫 로딩시 모든 캐릭터 정보를 Sqlite 에 저장, 이후 Sqlite 에서 모두 불러옴 (CSV기반 데이터만)
- 캐릭터 CSV 확인시, 파일이 변경되었을 경우엔 기존에 저장된 해당 번호의 캐릭터 정보만 갱신함
- exe와 동일한 위치의 emuera.db 에 저장되므로 CSV에 대량의 변화가 생겼을 경우 해당 db 파일을 삭제, 재실행하여 재구축 가능
- 옵션값 キャラクターチェック無視 를 통해 캐릭터 CSV를 불러오는 과정을 모두 건너뛸 수 있음 (로딩 속도 향상)
    YES : 건너뜀, NO : 캐릭터 CSV 확인함

- EmueraEE 기능 지원 (EmueraEE_readme.txt 참고)
- ezEmuera 기능 지원
- 옵션값 ezEmueraIsRun 으로 ezEmuera 기능 제어 가능. NO 로 하면 ezEmuera 기능을 끄고 쓸 수 있음.

[emuera.config 입력 방법]
1. emuera.config 를 Shift-JIS 인코딩으로 열고 아래 내용을 최하단에 입력. 이미 있는 경우는 값만 변경.

イメージチェック無視:YES
キャラクターチェック無視:YES
ezEmueraIsRun:YES

[기타 팁]
- 첫 실행후 db 파일이 만들어진 다음 위의 옵션을 config에 넣고 재실행하면 빠르게 로딩함
- CSV 수정 후엔 필히 한 번은 위의 옵션 중 キャラクターチェック無視 를 NO로 설정하고 실행해야함
- 대량의 캐릭터 CSV (Chara~~~~.csv) 파일이 고쳐졌을 경우엔 emuera.db 파일을 삭제 후 재실행하는 것이 확실함
- 배포는 대부분 텍챈(https://arca.live/b/textgame/)을 통해 진행함