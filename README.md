
`Firebase Studio`에 현 저장소를 Import합니다. (안드로이드 개발옵션 체크 필요)

임포트 완료후 아래 명령어로 빌드 및 실행해봅니다.

```bash
dotnet workload restore
dotnet build -f net9.0-android -t:InstallAndroidDependencies -p:AndroidSdkDirectory=/home/user/.androidsdkroot -p:AcceptAndroidSdkLicenses=True
dotnet build -f net9.0-android
dotnet build -f net9.0-android -t:Run
```