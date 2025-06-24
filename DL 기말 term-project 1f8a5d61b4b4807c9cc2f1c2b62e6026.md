# DL 기말 term-project

<aside>

💡 **목표: Icon Detector & Descriptor: 실제 + 가상 데이터를 활용한 UI 요소인식 및 설명 프로젝트**

- 사용 데이터:
    - **Synthetic UI 데이터** → 학습용
    - **실제 UI 캡처 이미지 40장** → 평가용 (직접 수집 + 라벨링 필요)
- 설명 생성: **BLIP 등 Pre-trained Vision-Language 모델** 활용 (학습 X)

5/22까지 - test set 만들기 

5/25까지 - train set 생성

5/28까지 - train set YOLO에 넣어보기

6/6까지 - 제출할 test set 준비

6/8까지 - BLIP 오류 원인 분석 + CLIP code 까지 짜보기 (더 효율적인 모델 찾기)

</aside>

[발표자료](https://www.notion.so/21ba5d61b4b480639df1c133d5c53daa?pvs=21)

---

## 1. test set 수집

[이미지 수집 및 라벨링(test set)](https://www.notion.so/test-set-1f8a5d61b4b480c68d83f4e955235870?pvs=21)

## 2. 가상 train set 생성

[Synthetic UI 데이터 생성(train set)](https://www.notion.so/Synthetic-UI-train-set-1f8a5d61b4b480d6ab9bf466a40548f7?pvs=21)

## 3. 모델 학습

[YOLO](https://www.notion.so/YOLO-1f8a5d61b4b480f4934df4dba8baff3d?pvs=21)

## 4. 설명 생성

[VLM](https://www.notion.so/VLM-1ffa5d61b4b480ddbcb0f81e357241b8?pvs=21)

---

### YOLO code

프로젝트를 위한 스터디

---

[김규림](https://www.notion.so/1f8a5d61b4b4803cbeb6e0f4b538b3a8?pvs=21)

[강다영](https://www.notion.so/201a5d61b4b48094bee6e7f46d531bde?pvs=21)

[서가영](https://www.notion.so/216a5d61b4b4804aa4e3c4188da9a229?pvs=21)

### model

프로젝트에 이용할 후보 모델 정하기

---

[BLIP](https://www.notion.so/BLIP-1f8a5d61b4b48010beafdf36fb804d08?pvs=21)

[CLIP](https://www.notion.so/CLIP-208a5d61b4b480e8b136e2ccf3ab183d?pvs=21)

# +) 서가영_결과

[test_set.json](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/instances_default.json)

[train_set.json](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/instances_default%201.json)

(train_set)

[image1](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.32.26_PM.png)

[image2](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.32.53_PM.png)

[image3](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.33.28_PM.png)

[image4](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.33.54_PM.png)

[image5](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.34.19_PM.png)

[image6](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.34.43_PM.png)

[image7](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.35.18_PM.png)

[image8](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.35.44_PM.png)

[image9](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.36.17_PM.png)

[image10](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.36.45_PM.png)

[image11](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.37.08_PM.png)

[image12](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.37.28_PM.png)

[image13](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.37.49_PM.png)

[image14](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.38.12_PM.png)

[image15](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.38.31_PM.png)

[image16](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.38.57_PM.png)

[image17](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.39.21_PM.png)

[image18](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.39.42_PM.png)

[image19](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.40.01_PM.png)

[image20](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.40.20_PM.png)

[image21](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.40.39_PM.png)

[image22](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.41.01_PM.png)

[image23](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.41.23_PM.png)

[image24](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.41.41_PM.png)

[image25](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.42.01_PM.png)

[image26](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.42.22_PM.png)

[image27](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.42.42_PM.png)

[image28](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.43.02_PM.png)

[image29](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.43.22_PM.png)

[image30](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/Screenshot_2025-05-23_at_4.43.41_PM.png)

[instances_default.json](DL%20%E1%84%80%E1%85%B5%E1%84%86%E1%85%A1%E1%86%AF%20term-project%201f8a5d61b4b4807c9cc2f1c2b62e6026/instances_default%202.json)

# Streamlit 아이디어 : streamlit 버튼 기능을 활용해 데이터 불러오기 구현하여 결과 발표

Streamlit은 무엇을 하나요?

Streamlit은 HTML, CSS, JavaScript 없이도 **Python 스크립트를 아름답고 인터랙티브한 웹 앱으로 바꿔주는 도구**입니다.

예를 들어, 데이터 시각화나 머신러닝 모델을 사용하는 Python 코드를 가지고 있다면, 몇 가지 Streamlit 명령만 추가해도 슬라이더, 드롭다운, 버튼, 실시간 차트 같은 UI를 손쉽게 만들 수 있습니다.

### 🎚️ 1. **슬라이더 (Slider)**

**모습:**

- 숫자를 조절할 수 있는 바 형태
- 마우스로 드래그하거나 클릭해서 값 조정
- 예시: 음량 조절, 숫자 범위 선택 등

### 2. **드롭다운 (Dropdown / Selectbox)**

**모습:**

- 클릭 시 목록이 펼쳐짐
- 하나의 항목만 선택 가능
- 예시: 카테고리 선택, 설정 등

### 3. **버튼 (Button)**

**모습:**

- 클릭 가능한 직사각형 형태
- 클릭 시 이벤트 발생
- 예시: 모델 실행, 데이터 불러오기 등

### 4. **실시간 차트 (Real-time Chart)**

**모습:**

- 실시간으로 업데이트되는 선 그래프
- `a`, `b`, `c` 값의 변화 시각화
- 예시: 센서 데이터, 모델 결과 변화 등

# 데이터 증강

## ✅ 요약: "이미지 없이 YOLO .txt 라벨만 증강하기"

- YOLO의 라벨 포맷은 `class_id x_center y_center width height`
- 이 모든 값은 **이미지 크기에 대해 정규화된 값(0~1)**이므로,
- **이미지가 없어도 일부 증강(좌우반전, 이동, 확대 등)은 가능**합니다.

---

## ⚠️ 가능/불가능한 증강 요약

| 증강 종류 | 가능 여부 | 비고 |
| --- | --- | --- |
| 좌우반전 (flip) | ✅ 가능 | x 좌표만 반전 |
| 위아래반전 (flip) | ✅ 가능 | y 좌표만 반전 |
| 위치 이동 | ✅ 가능 | 범위 설정 필요 |
| 스케일 변경 | ✅ 가능 | width/height 변화 |
| 회전 | ❌ 어려움 | 이미지 없이 회전은 정확하지 않음 |
| 밝기/색상 변화 | ❌ 불가능 | 이미지 필요 |

🛠️ 실전 예제: YOLO .txt만 증강하기 (Colab/로컬 가능)

```jsx
import os
import random

input_dir = "labels"  # 원본 .txt 라벨 폴더
output_dir = "augmented_labels"  # 증강된 라벨 저장할 폴더
os.makedirs(output_dir, exist_ok=True)

def flip_horizontal(bbox):
    # 좌우 반전: x_center만 반전
    return [bbox[0], 1 - bbox[1], bbox[2], bbox[3]]

def flip_vertical(bbox):
    # 상하 반전: y_center만 반전
    return [bbox[0], bbox[1], bbox[2], 1 - bbox[3]]

def shift_bbox(bbox, dx=0.05, dy=0.05):
    # 박스 위치 이동 (x/y에 ±dx/dy만큼 이동)
    return [min(max(bbox[0] + dx, 0), 1),
            min(max(bbox[1] + dy, 0), 1),
            bbox[2],
            bbox[3]]

def scale_bbox(bbox, sx=1.1, sy=1.1):
    # 박스 크기 확대/축소
    return [bbox[0], bbox[1],
            min(bbox[2] * sx, 1),
            min(bbox[3] * sy, 1)]

# 모든 .txt 파일에 대해 처리
for file_name in os.listdir(input_dir):
    if not file_name.endswith(".txt"):
        continue

    with open(os.path.join(input_dir, file_name), "r") as f:
        lines = f.readlines()

    augmented_lines = []

    for line in lines:
        parts = line.strip().split()
        cls = parts[0]
        bbox = list(map(float, parts[1:]))

        # 랜덤하게 증강 선택
        aug_type = random.choice(['flip_x', 'flip_y', 'shift', 'scale'])

        if aug_type == 'flip_x':
            bbox = flip_horizontal(bbox)
        elif aug_type == 'flip_y':
            bbox = flip_vertical(bbox)
        elif aug_type == 'shift':
            bbox = shift_bbox(bbox, dx=random.uniform(-0.05, 0.05), dy=random.uniform(-0.05, 0.05))
        elif aug_type == 'scale':
            bbox = scale_bbox(bbox, sx=random.uniform(0.8, 1.2), sy=random.uniform(0.8, 1.2))

        augmented_lines.append(f"{cls} {' '.join(map(str, bbox))}\n")

    with open(os.path.join(output_dir, f"{file_name.replace('.txt', '')}_aug.txt"), "w") as f:
        f.writelines(augmented_lines)

```