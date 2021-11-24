# AIhub Dataset + mobileNetV3
AI hub 대회 사용한 MobileNetV3모델의 코드를 올리고 [AI허브](https://aihub.or.kr/) 생활폐기물 데이터셋으로 학습된 pre-trained weight를 제공합니다.


# AI허브 생활폐기물 데이터셋 정보
[다운로드 링크](https://aihub.or.kr/aidata/27708)
- 전체 이미지수 : 36713
- 클래스 종류 : 49가지
![2](https://user-images.githubusercontent.com/41135138/143242706-762b1694-a631-4b5d-8717-85d9a1980bea.PNG)

# Data Statistics
| Class | # | Class | # |
|-----------------|------|----------------------|------|
| Meal_award(밥상) | 828 | Chest_drawers(서랍장) | 1095 |
| Storage_closet(수납장)| 1001 | Sink(싱크대) | 31 |
| Dish_dryer(식기건조기) | 111 | Chair(의자) | 1351 |
| Wardrobe(장롱) | 566 | 책상(Desk) | 1621 |
| Bed(침대) | 60 | scrap_metal(고철) | 1006 |
| Golf_club(골프채) | 1000 | Electronic_frying_pan(전기 프라이팬) | 206 |
| Pottery_kettle(도기류-주전자) | 169 | Chair_sofa(의자형 소파) | 530 |
| Hanger(철옷걸이) | 986 | Frying_pan(프라이팬) | 1000 |
| Sofa(소파) | 807 | Wooden_hanger(나무행거) | 390 |
| Printer(프린터) | 1015 | Refrigerator(냉장고) | 1015 |
| Computer(컴퓨터) | 1015 | TV(티비) | 1015 |
| Washing_machine(세탁기) | 455 | Vacuum_cleaner(청소기) | 1000 |
| Air_conditioner(에어컨) | 180 | Food_dispenser(음식물처리기) | 76 |
| Audio(오디오) | 1040 | Electric_iron(전기다리미) | 913 |
| Copy_machine(복사기) | 305 | Video_player(비디오플레이어) | 790 |
| Mixer(믹서) | 932 | Electric_water_purifier(전기정수기) | 330 |
| Electric_heater(전기히터) | 1000 | Electric_rice_cooker(전기밥솥) | 1000 |
| Electric_oven(전기오븐) | 1000 | Microwave(전자레인지) | 550 |
| Humidifier(가습기) | 560 | box(상자) | 1015 |
| Tricycle(세발자전거) | 407 | Four-wheeled-bicycle(네발자전거) | 1000 |
| Bottom(하의) | 1000 | Coat(외투) | 1014 |
| One_piece(원피스) | 1014 | Water_softener(연수기) | 1014 |
| Booklets(책자) | 1000 | Frame(액자) | 1000 | 
| Chopping_board(도마) | 1015 | Facsimile(팩시밀리) | 145 |
| Scrap_metal_kettle(고철류-주전자) | 529 | Bicycle(두발자전거) | 1006 |
| Phone(핸드폰) | 1040 | Electric_fan(선풍기) | 1013 |
| Clothing(면의류) | 132 | Iron_hanger(철옷걸이) | 986 |
| High_pass(하이패스) | 21 |
# Training Model
## 1.DATASET 구성
<pre><code>	    
--Training
  |--Meal_award
  |  |--imgname.jpg
  |  |--imgname.jpg
  |  |--imgname.jpg
  |  |--imgname.jpg
  |  |-- ...
  |-- Chest_drawers
  |  |--imgname.jpg
  |  |--imgname.jpg
  |  |--imgname.jpg
  |  |--imgname.jpg
  |  |-- ...
 </code></pre>
## 2. 학습
MobileNetV3 -> jupyter notebook
model.fit()
![5](https://user-images.githubusercontent.com/41135138/143243084-0cbb7667-3c4b-4b24-9793-fef1deda4c32.PNG)
![6](https://user-images.githubusercontent.com/41135138/143243296-9d200274-1de2-4274-bd7f-070d2e11e96d.PNG)


## 3.학습 loss, Accuracy
![download](https://user-images.githubusercontent.com/41135138/143243248-2567041f-5fc1-4fc8-b7e8-12c5dc79ce62.png)

# MobileNet Models
- MobileNetLargeV3 Trained with 49 class -> MobileNetLargeV3.h5
- MobileNetSMALLV3 Trained with 49 class -> MobileNetSMALLV3.h5
