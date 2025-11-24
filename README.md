# MarisaReturnTheBook_TranslateKR
마리사 책 돌려줘!의 한국어 재번역본입니다.

번역은 일부 의역이 있으며 Ai를 중간중간 사용하였기에 검수 못한 부분이 있을 수 있습니다.

번역파일을 직접 패치해야하니 순서에 맞게 따라해주시면 됩니다.

## 준비물
1. 게임원본(스팀버전)
2. DnSpy [[다운링크](https://github.com/dnSpyEx/dnSpy/releases/tag/v6.5.1)]
3. 프로젝트 번역파일(복사 혹은 다운받기)
(.cs 파일은 .txt로 바꿔 열어도 문제 없습니다)
 
## 패치방법
1. DnSpy를 실행합니다

2. 상단 File의 Open을 눌러줍니다.
<img width="1288" height="716" alt="image" src="https://github.com/user-attachments/assets/33d4b537-73f9-4543-ab76-3b81232d5ee8" />

3.  "\SteamLibrary\steamapps\common\Marisa!ReturnTheBook!\Marisa!ReturnTheBook!\MarisaReturnTheBook_Data\Managed"에 Assembly-CSharp.dll을 열어줍니다 (해당 위치는 조금씩 다를 수 있습니다)

<img width="716" height="162" alt="image" src="https://github.com/user-attachments/assets/1876ce9b-1bf7-445c-9527-ca098053ea17" />
4. 다음과 같은 순서로 경로를 열어 해당 위치까지 접근합니다.

- Assembly-CSharp(0.0.0.0)[최상위 부모]
  - Assembly-CSharp.dll
    - {}-
      - TextManager @0200005C
        - GetDataByKR():void @060002E4

5. 상단 Edit - Edit Method(C#)을 눌러 창을 띄워 줍니다.
<img width="1290" height="715" alt="image" src="https://github.com/user-attachments/assets/838c2ec2-163f-4b48-ae13-408bf8af49c8" />

6. 이 프로젝트에 첨부된 번역본을 복사하여 전체 붙여넣기를 한뒤 Compile버튼을 눌러줍니다

7. 상단 File - Save all을 눌러 줍니다. 
<img width="310" height="401" alt="image" src="https://github.com/user-attachments/assets/5a617978-6b7e-408b-9a2a-2d8ad2163d63" />

8. 해당창이 뜨면 OK를 눌러주시면 패치가 완료됩니다. (완료된 후엔 DnSpy를 삭제해도 무방합니다)
<img width="492" height="444" alt="image" src="https://github.com/user-attachments/assets/6f6612cb-7c94-4d3b-a7e8-48120c5b9386" />

---

문제가 있거나 번역 개선방향이 있다면 존재한다면 이슈에 글을 써주세요!

version 1.00을 기준으로 작성되었습니다. 업데이트시 문제가 있을 수 있습니다.
