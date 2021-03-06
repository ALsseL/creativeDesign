# 정의
  ## 용도
  - 플레이어가 게임 중에 사용할 수 있는 무기를 정리해 놓음
  - 일부 총기에는 스킨 적용이 가능

  ## 기대효과
  - 게임 플레이 중에 직접적으로 확인하기 힘든 수치를 간단한 그래프로 확인
  - 무기에 부착물을 적용한 외관을 확인 가능
<br>
<br>

# 구성도
![무기고](./Resource/view11.png)
<br>
<br>

# 인터페이스 페이지 세부요소
  ## 배경이미지 (Element-00)
    - 전체적으로 검은 배경에 하단이 붉은 이미지
    - 밑에서 불에서 불꽃이 튀는 듯한 애니메이션
  ## 무기 설명 (Element-01)
    - 무기의 간단한 정보를 설명하는 요소
    - 무기의 이름과 간단한 설명이 있고, 총기의 경우 사용 탄약이 적혀있음
  ## 무기 성능 그래프 (Element-02)
    - 전투력 등의 무기 수치를 그래프화
  ## 무기 선택 버튼 (Element-03)
    - 무기의 종류와 해당하는 무기를 선택할 수 있음
    - 여기서 선택한 무기를 나머지 요소를 통해 보여줌
  ## 총기 3D 오브젝트 (Element-04)
    - 총기의 외관을 볼 수 있는 오브젝트
    - 기본적으로 수평방향으로 회전하고 있음
    - 화면 터치를 통해 회전을 멈추거나 조절할 수 있음
  ## 스킨 및 부착물 버튼 (Element-05)
    - 무기에 달 수 있는 부착물들을 확인하고, 실제 장착한 외관을 확인할 수 있음
    - 무기의 능력이 변하는 부착물의 경우 Element-02에 그 변화가 나타남
    - 스킨이 있는 무기는 스킨을 적용해볼 수 있음
  ## 화면 조작 버튼 (Element-06)
    - 06-1 : 총기의 회전을 초기화시키는 버튼
    - 06-2 : 총기 오브젝트를 제외한 다른 요소를 안보이게 함
             이 경우 화면 우상단에 생기는 X 버튼을 터치하면 다시 돌아옴
<table>
  <thead>
    <tr>
      <th colspan=3> 총기 상세 능력 표
    </tr>
    <tr>
      <th> <a href="./Resource/무기고/AR/무기고-AR.md"> AR
      <th> <a href="./Resource/무기고/SMG/무기고-SMG.md"> SMG
      <th> <a href="./Resource/무기고/SR/무기고-SR.md"> SR
    </tr>
    <tr>
      <th> <a href="./Resource/무기고/DMR/무기고-DMR.md"> DMR
      <th> <a href="./Resource/무기고/SG/무기고-SG.md"> SG
      <th> <a href="./Resource/무기고/LMG/무기고-LMG.md"> LMG
    </tr>
</table>
<br>
<br>


# 기능흐름
  - 무기 선택 버튼
    - 화면이 그 무기에 해당하는 요소들로 변경
  - 버튼을 제외한 화면 전체
    - 터치와 드래그를 통해 총기 회전을 제어 가능
  - 스킨 및 부착물 버튼
    - 선택한 내용에 따라 무기 오브젝트의 외관이 바뀜
  - 회전 초기화 버튼
    - 자유롭게 바꾸었던 총기의 회전을 초기화 함
  - 확대 버튼
    - 총기 오브젝트 이외의 UI를 안보이게 함
    - 화면 우상단에 X 표시를 누르면 원상태로 돌아옴
