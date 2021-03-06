# 변수명 정리표

* ## 1. 기본 변수
    - ### 1. 시스템
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 명령어 입력 | cmdInput | `str` | |
      | 함수 로직 판단 | funcLogic | `int` | `0`: 문제없음, `1` : 입력 오류, `2`: 치명적인 오류 |
      | 오류문 출력 | strError | `str` | `다시 입력해주세요.` |
      | 게임 페이지 | page | `str` | `mainPage` : 게임 첫 화면,  `characterGeneration` : 캐릭터 생성, `prologue` : 프롤로그, `inGame` : 인게임 |
      | 게임 세부 페이지 | advPage | `str` | |
      | 프롤로그 스토리 문자열 | strPrologue | `str` | |
      | 문자열 | strs | `str` | 문자열 출력 함수에 사용 |
      | 지연시간 | timeDelay | `int` | 기본값: `0.045` |
      | 진행도 | progress | `int` | 메인 퀘스트 클리어 갯수 |

* ## 2. 플레이어 관련 변수
    - ### 1. 스텟 관련
        + #### 1. 기본 스텟 관련
          | 이름 | 변수명 | 타입 | 특이사항 |
          | :---: | :---: | :---: | :---: |
          | 플레이어 기본 공격력 | playerBasicAtk | `int` | 초기값: `5` |
          | 플레이어 기본 방어력 | playerBasicDef | `int` | 초기값: `5` |
          | 플레이어 기본 민첩성 | playerBasicAgi | `int` | 초기값: `50%` |
          | 플레이어 기본 정확도 | playerBasicAcc | `int` | 초기값: `50%` |
          | 플레이어 기본 체력 | playerBasicHP | `int` | 초기값: `100` |
          | 플레이어 기본 스태미나 | playerBasicStm | `int` | 초기값: `50` |
          | 플레이어 기본 스텟 관련 딕셔너리 | dictPlayerBasicStat | `dict` | |
          
        + #### 2. 최종 스텟 관련
          | 이름 | 변수명 | 타입 | 특이사항 |
          | :---: | :---: | :---: | :---: |
          | 플레이어 최종 공격력 | playerAtkAP | `int` | |
          | 플레이어 최종 방어력 | playerTotalDef | `int` | |
          | 플레이어 최종 민첩성 | playerTotalAgi | `int` | |
          | 플레이어 최종 정확도 | playerTotalAcc | `int` | |
          | 플레이어 최종 체력 | playerTotalHP | `int` | |
          | 플레이어 최종 스태미나 | playerTotalStm | `int` | |
          | 플레이어 최종 데미지 | playerTotalDmg | `int` | |
          | 플레이어 최종 회피율 | playerTotalAvd | `int` | |
          | 플레이어 최종 선공확률 | playerTotalFatk | `int` | |
          | 플레이어 최종 퇴각확률 | playerTotalFlee | `int` | |
          | 플레이어 최종 스텟 관련 딕셔너리 | dictPlayerStat | `dict` | |

        + #### 3. 스텟 포인트로 증가한 포인트 관련
          | 이름 | 변수명 | 타입 | 특이사항 |
          | :---: | :---: | :---: | :---: |
          | 플레이어 공격력 증가량 | playerAtkAP | `int` | |
          | 플레이어 방어력 증가량 | playerDefAP | `int` | |
          | 플레이어 민첩성 증가량 | playerAgiAP | `int` | |
          | 플레이어 정확도 증가량 | playerAccAP | `int` | |
          | 플레이어 체력 증가량 | playerHPAP | `int` | |
          | 플레이어 스태미나 증가량 | playerStmAP | `int` | |
          | 플레이어 스탯 포인트 관련 딕셔너리 | dictPlayerStatAP | `dict` | |
          
        + #### 4. 기타
          | 이름 | 변수명 | 타입 | 특이사항 |
          | :---: | :---: | :---: | :---: |
          | 플레이어 추가 공격력 % | playerAddAtk | `int` | |

    - ### 3. 스텟 포인트, 스킬 포인트 관련
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 플레이어 스텟 포인트 | playerAP | `int` | `초기값: 2` |
      | 플레이어 스킬 포인트 | playerSP | `int` | |
      | 플레이어 스텟 포인트, 스킬 포인트 관련 딕셔너리 | dictPlayerPoint | `dict` | |
    
    - ### 4. 레벨 관련
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 플레이어 레벨 | playerLv | `int` | 초기값: `1` |
      | 플레이어 경험치 | playerExp | `int` | |
      | 필요 경험치 | reqExp | `int` | 초기값: `14` |
      | 플레이어 레벨 관련 딕셔너리 | dictPlayerLv | `dict` | |
      
    - ### 5. 플레이어 기본 정보 관련
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 플레이어 이름 | playerName | `str` | 1 ~ 12 글자 영문 (공백 없음) |
      | 플레이어 직업 | playerJob | `str` | 시작 직업: `견습생` |
      
    - ### 6. 플레이어 장비 관련
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 플레이어 무기 | playerWeapon | `dict` |  |
      | 플레이어 헬멧 | playerHelmet | `dict` |  |
      | 플레이어 방탄복 | playerVest | `dict` |  |
      | 플레이어 부츠 | playerBoots | `dict` |  |
      | 플레이어 탄약 | playerAmmo | `int` |  |
      | 플레이어 장비 딕셔너리 | dictPlayerEquip | `dict` | |
      
    - ### 7. 플레이어 아이템 관련
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 플레이어 아이템 보관함 | listPlayerItemSpace | `list` |  |
      
    - ### 8. 플레이어 스킬 관련
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 플레이어 스킬 보관함 | listPlayerSkillSpace | `list` |  |
      
* ## 3. 장비 관련 변수
    - ### 1. 무기 관련 변수
        + #### 1. 권총
          | 이름 | 변수명 | 타입 |
          | :---: | :---: | :---: |
          | null | dictWeaponPistolNull | `dict` |
          | USP | dictWeaponPistolUSP | `dict` |
          | Glock-19 | dictyWeaponPistolGlock19 | `dict` |
          | M1911 | dictWeaponPistolM1911 | `dict` |
          | HK45 | dictWeaponPistolHK45 | `dict` |

        + #### 2. 돌격소총
          | 이름 | 변수명 | 타입 |
          | :---: | :---: | :---: |
          | null | dictWeaponRifleNull | `dict` |
          | M16A4 | dictWeaponRifleM16A4 | `dict` |
          | G36A3 | dictWeaponRifleG36A3 | `dict` |
          | HK416 | dictWeaponRifleHK416 | `dict` |

        + #### 3. 산탄총
          | 이름 | 변수명 | 타입 |
          | :---: | :---: | :---: |
          | null | dictWeaponShotgunNull | `dict` |
          | Winchester M1897 | dictWeaponShotgunWinchesterM1897 | `dict` |
          | Remington 870 | dictWeaponShotgunRemington870 | `dict` |
          | Benelli M4 S90 Tectical	 | dictWeaponShotgunBenelliM4S90Tectical | `dict` |

        + #### 4. 저격소총
          | 이름 | 변수명 | 타입 |
          | :---: | :---: | :---: |
          | null | dictWeaponSniperNull | `dict` |
          | M40 | dictWeaponSniperM40 | `dict` |
          | K14 | dictWeaponSniperK14 | `dict` |
          | M82	 | dictWeaponSniperM82 | `dict` |

    - ### 2. 방어구 관련 변수
        + #### 1. 헬멧
          | 이름 | 변수명 | 타입 |
          | :---: | :---: | :---: |
          | null | dictHelmetNull | `dict` |
          
        + #### 2. 방탄복
          | 이름 | 변수명 | 타입 |
          | :---: | :---: | :---: |
          | null | dictVestNull | `dict` |
          
        + #### 3. 부츠
          | 이름 | 변수명 | 타입 |
          | :---: | :---: | :---: |
          | null | dictBootsNull | `dict` |

* ## 4. 스킬 관련 변수
    - ### 1. 견습생
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 더블 파이어 | dictSkillNoviceDoubleFire | `dict` |  |
      
    - ### 2. 소총수
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 소총 난사 | dictSkillRiflemanBulletSpray | `dict` |  |
      
    - ### 3. 돌격병
      | 이름 | 변수명 | 타입 | 특이사항 |
      | :---: | :---: | :---: | :---: |
      | 산탄총 연사 | dictSkillStormtrooperDoubleShot | `dict` |  |
