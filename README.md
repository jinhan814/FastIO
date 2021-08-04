# FastIO

## FastIO implementation for cin, cout.

c++의 cin, cout을 대체해 사용할 수 있는 빠른 입출력 구현 코드입니다. 위 코드를 **복사 붙여넣기**만 하시면 cin, cout이 mmap, write로 구현된 빠른 입출력 함수로 대체됩니다.

(참고 : [https://www.acmicpc.net/blog/view/105](https://www.acmicpc.net/blog/view/105), [https://blog.naver.com/jinhan814/222400578937](https://blog.naver.com/jinhan814/222400578937))

## Update Log.

* 21-03-06 : >>, << operator 구현
* 21-03-18 : 구분선 추가, cin의 explicit opertor bool() 구현
* 21-03-22 : class를 이용해 다시 구현, getline 구현
* 21-04-14 : template를 이용해 >>, << operator가 모든 자료형을 처리할 수 있도록 수정, 구현 더 간단하게 수정.
* 21-04-14 : BOJ 게시판에 설명글 작성 ([참고](https://www.acmicpc.net/blog/view/105))
* 21-04-16 : SFINAE를 이용해 >>, << operator 오버로딩 보완
* 21-05-05 : cout의 explicit operator bool() 구현, ReadInt, WriteInt에서 비트 연산을 이용해 성능 개선
* 21-05-06 : mmap에서 fstat을 이용해 INPUT_SZ를 지정하지 않고 알아서 stdin의 크기를 받아오도록 수정
* 21-06-16 : 구현 원리 글 작성 ([참고](https://blog.naver.com/jinhan814/222400578937))
* 21-07-22 : Jinhan's Note / 알고리즘 가이드 - fastio 글 작성 ([참고](https://blog.naver.com/jinhan814/222440944366))