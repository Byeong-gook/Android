## Toast를 활용해 알림창 띄워보기 

onclick : 버튼이 클릭 되었을때 실행할 함수 이름 넣어주기

버튼 컴포넌트 하나 만든 후 Common Attributes에  onClick 속성값에 onButton1Clicked 속성값 부여

```
//onButton1Clicked 함수 정의
public void onButton1Clicked(View v) {
    Toast.makeText(this, "확인1 버튼이 눌렸어요", Toast.LENGTH_LONG).show();
}
```



버튼 컴포넌트 하나 만든 후 Common Attributes에  onClick 속성값에 onButton2Clicked 속성값 부여

## 네이버 접속하기 버튼

```
public void onButton2Clicked(View v) {
    Intent intent = new Intent(Intent.ACTION_VIEW, Uri.parse("http://m.naver.com"));
    startActivity(intent); // 함수 실행 startActivity
}
```



버튼 컴포넌트 하나 만든 후 Common Attributes에  onClick 속성값에 onButton3Clicked 속성값 부여



## 전화걸기 버튼 

```
public void onButton3Clicked(View v) {
    Intent intent = new Intent(Intent.ACTION_VIEW, Uri.parse("tel:010-5628-7173"));
    startActivity(intent);
}
```