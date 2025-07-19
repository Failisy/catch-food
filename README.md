플레이어는 허기 버프를 가진 상태로 가장 오래 버티기 위해 주변에서 생성되는 음식을 먹으며 버티는 게임입니다.

플레이어 주변 표면에 랜덤으로 음식과 공격 아이템을 소환합니다.

투척용 허기의 물약(공격 아이템): 맞은 대상의 허기를 4칸을 소모시킵니다.

CF.config 스코어보드로 게임룰을 설정할 수 있습니다  
`/scoreboard players set <name> CF.config <score>`  
name 목록  
> spawnDelaySec       : 음식이 소환되는 시간 초를 설정합니다. {init: 3}  
> spawnRadiusChunks   : 음식이 소환되는 청크 범위를 설정합니다. (init: 1)  
> spawnFood           : 음식의 소환 여부를 결정합니다 (boolean)  
> hunger              : 전체 플레이어에게 허기 버프를 부여합니다. (boolean)'  

`/function catch_food:recommend`  : 게임에서 지정한 권장 설정을 불러옵니다.  
(spawnFood: 1, hunger: 1, naturalRegeneration: false, 전체 플레이어의 체력과 허기 회복)  
`/function catch_food:disable/`    : 모든 기능을 비활성화합니다.

`*catch_food/tags/items/food.josn` 파일을 수정하여 음식 목록을 수정할 수 있습니다.

추천 추가 설정  
    해당 데이터팩을 미니게임 형식으로 즐기기 위해서는 아래 명령어를 통해 맵 크기를 제한하시는 걸 추천드립니다.  
`/worldborder center <x> <z>
/worldborder set <distance> <second>`
