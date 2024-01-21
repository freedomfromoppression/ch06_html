# ch06_html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>tag에 javascrip 작성</title>
</head>
     
<body>
    <h3>마우스를 이미지에 올려보세요</h3>
    
        <img src="./img/apple.PNG" onmouseover="this.src='./img/banana.PNG'" onmouseout="this.src='./img/apple.PNG'" >
        
  
    
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script>
        function fn_over(obj){
            obj.sec='./img/banana.PNG';
        }
        function fn_out(obj){
            obj.src='./img/apple.PNG';
        }
    </script>
</head>
<body>
    <img src="./img/apple.PNG"alt="" onmouseover="fn_over(this)"
              onmouseout="fn_out(this)">
             
             
             
    
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>if-else</title>
</head>
<body>
    <h3>if_else 를 이용한 학점 출력</h3>
    <hr>
    <!-- script 태그는 html 문서 어디서든 사용가능(여러개도 괜찮음)-->
    <script>
        let grade;
        //사용자 입력은 기본 string
        let score = prompt("점수를 입력하세요");
        //score 변수가 최초 strong 이였지만 int 형태로토 받아드림
        score=prompt(score); // 정수형태로 타입변환
        if(score>=90){
            grade="A";
        }else if(score>=80){
            grade="B";
        }else{
            grade="F";
        }
        document.write(score + "는" + grade+"입니다.");
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>for문 css변경</title>
</head>
<body>
    <h3>for 문으로 10xp~35px 크기 텍스트 출력</h3>
    <hr>
    <script>
        for(let i= 10; i<=35; i+5){
            document.write("<span ");
            document.write("style='font-size:" +i
            + "px; color:rgb("+(i * 2)+","+(i * 5)+","+(i * 6)+");'>");
            document.write(i +"px");
            document.write("</span><br>");
}
    </script>
    
</body>
</html>
