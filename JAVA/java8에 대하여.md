JAVA8 변경사항

	1. 
람다 표현식 : 함수형 프로그래밍
	2. 
스트림API : 데이터의 추상화
	3. 
java.time 패키지 : Joda-Time을 이용한 새로운 날짜와 시간 API
	4. 
나즈혼 : 자바스크립트의 새로운 엔진




	1. 
람다 표현식


            식별자 없이 실행할 수 있는 함수 표현식을 의미하며 익명 함수 라고도 부른다.
            
    
        2. 스트림 API 자바에서는 많읜 양의 데이터를 저장하기 위해서 배열이나 컬렉션을 사용합니다.
            이렇게 저장된 데이터에 접근하기 위해서는 반복문이나 반복자를 이용하여 매번 코드를 작성해야 했습니다.
            이를 극복하기 위하여 스트림 사용
            
            String[] arr = new String[]{"넷", "둘", "셋", "하나"};
 
       // 배열에서 스트림 생성
        Stream<String> stream1 = Arrays.stream(arr);
        stream1.forEach(e -> System.out.print(e + " "));
        System.out.println();
 
        // 배열의 특정 부분만을 이용한 스트림 생성
        Stream<String> stream2 = Arrays.stream(arr, 1, 3);
        stream2.forEach(e -> System.out.print(e + " "));