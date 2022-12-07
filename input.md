```javaScript
    const [title, setTitle] = useState("")

  // 기능 작성
    const inputTitle = (e) => {
      console.log(e.target);          // 출력 : <input type="text" name="title" value="ㅋㅋㅋ">
      console.log(e.target.value)     // 출력 : ㅋㅋㅋ
      setTitle(e.target.value);
    };

  // 내가 input에 작성한 "ㅋㅋㅋ"은 "value"안에 들어있다는 사실을 콘솔로 확인할 수 있다.
  // 결국 ㅋㅋㅋ은 title로 저장된다.

  // jsx 작성
  <input type="text" name="title" value={title} onChange={inputTitle} />
```
