# 유니티 개념 정리

 **- 1주차. 유니티 물리와 뉴 인풋 시스템**
     - RigidBody2D -> 유니티 2D 물리(속도,힘 등), 중력이 적용됨 , Constraints 가서 Freeze Rotation 해주면 흔들리지 않고 떨어짐
     - BoxCollider2D -> 2D 충돌 처리

 **- 유니티 생명 주기**
     - 게임시작 -> Awake() -> Start() -> FixedUpdate(), Update() -> LateUpdate()
     - 오브젝트 활성화 시 -> OnEnable()
     - 오브젝트 비활성화 시 -> OnDisable()

- Update()
       - 입력 처리 등 
       - 매 프레임마다 호출
       - -> 불규칙한 호출 주기(프레임 호출에 따라 달라짐)

- FixedUpdate()
       - 고정된 시간마다 호출
       - 물리 연상 등 처리

- LateUpdate()
       - update()가 끝나면 호출
       - 후속 처리가 필요한 경우

  순서까지 정리하면
  ![image](https://github.com/user-attachments/assets/e4d645b3-a7dd-4b3d-a50a-9ca297fe04fc)

  그림으로 정리하자면
![image](https://github.com/user-attachments/assets/90298250-b2a8-4b47-a1d0-a58b96a0b066)

![image](https://github.com/user-attachments/assets/8ee8ac0f-339e-4798-a715-69b881c3d84c)

![image](https://github.com/user-attachments/assets/2581764a-6725-42f5-8b44-32de530dc806)

      각 Interaction은 매개변수를 줄 수 있음
       - 1초 이상 눌러야 작동 등.. (커스터마이징이 가능하다)
![image](https://github.com/user-attachments/assets/f4f82888-b490-4af2-b257-e4870165140b)

     
