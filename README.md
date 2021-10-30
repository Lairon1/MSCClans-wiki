![ЛОГО](https://github.com/Lairon1/MSCClans-wiki/blob/main/images/MSC.png)
# MSCClans
 Лучшие кланы для вашего сервера.
 При покупке плагина вы получаете пожизненную и бесплатную поддержку со стороны разработчика.
 По поводу покупки писать сюда - https://vk.com/mysouliscry
 ## Команды
 - [] - Не обязательный аргумент.
 - <> - Обязательный аргумент.
## Комманды для игроков

| Команда               |Назначение                       |Право                     |
|----------------|-------------------------------|-----------------------------|
|/clan create <ТЕГ>|Создать клан           |mscclans.clan.create            |
|/clan reload        |Перезагрузка конфигов         |mscclans.reload           |
|/clan disband         |Распустить клан | Для главы клана|
|/clan invite <НИК> |Пригласить игрока в клан           |Для модераторов клана и выше            |
|/clan accept <ТЕГ>         |Принять приглашение в клан          |-            |
|/clan kick <НИК>         |Исключить игрока из клана| Для модераторов клана и выше|
|/clan promote|Повысить участника клана до модератора           |Для главы клана            |
|/clan color <ЦВЕТ>          |Изменить цвет клана          |Для главы клана            |
|/clan sethome          |Поставить клановую базу| Для главы клана|
|/clan leave| Выйти из клана            |-           |
|/clan info [ТЕГ]       |Открыть GUI с информацией о клане           |-            |
|/clan give <НИК>         |Передать клан| Для главы клана|
|/ch [ТЕГ]|Телепорт на клановую базу          |-          |
|/clan setWelcome <СООБЩЕНИЕ>       |Назначить сообщение для клана            |Для главы клана            |
|/clan removeWelcome         |Удалить сообщение для клана| Для главы клана|
|/clan deleteHome|Удалить клановую базу            |Для главы клана           |
|/clan homeType        |Открыть/Закрыть клановую базу           | Для главы клана          |
|/clan deposit <СУММА>         |Пополнить банк клана|-|
|/clan take <СУММА>         |Снять с банка клана| Для главы клана|
|/clan pvptype         |Включить/выключить пвп в клане|Для главы клана|
|/clan allianceinvite <ТЕГ>        |Запросить союз кланов |Для главы клана|
|/clan allianceaccept <ТЕГ>        |Принять союз клана |Для главы клана|

## Комманды для администрации.(Право на все комманды "mscclans.clanadmin")
| Команда               |Назначение                       |
|----------------|-------------------------------|
|/clanadmin setholo <ГОЛОГРАММА>        |Установить голограмму|
|/clanadmin remholo <ГОЛОГРАММА>        |Удалить голограмму с топом по банку клана|
|/clanadmin disband <ТЕГ>      |Удалить любой клан|

## Доступные голограммы:

 1. Bank - топ по казне клана
 2. Exp - топ по опыту клана
 3. Level - топ по уровню клана
 4. Members - топ по участникам клана
![ТОПЫ КЛАНА](https://github.com/Lairon1/MSCClans-wiki/blob/main/images/holotop.png)
## GUI 
![GUI КЛАНА](https://github.com/Lairon1/MSCClans-wiki/blob/main/images/gui.png)
## Ивенты 
Для каждого ивента имеется своя шкала прогресса. После победы показывает победителя.
![PROGRESS BAR](https://github.com/Lairon1/MSCClans-wiki/blob/main/images/demonBAR.png)

![WIN BAR](https://github.com/Lairon1/MSCClans-wiki/blob/main/images/winBar.png)
### Красный демон
![enter image description here](https://github.com/Lairon1/MSCClans-wiki/blob/main/images/demonMOB.png)
#### Способности:
 ##### Режим ярости
Включается когда у демона остаётся меньше 300 HP и длится 10 секунд (Настраивается)
 В режиме ярости демон выбирает себе цель и начинает носится за ней нанося урон.
#####  Атака по радиусу
Демон наносит урон по игрокам в радиусе от него.
##### Ускорение
Демон выбирает цель, ускоряется в ее сторону и наносит урон.
##### Призыв друидов
Демон призывает вокруг друидов.
### Ведьма
![enter image description here](https://github.com/Lairon1/MSCClans-wiki/blob/main/images/mag.png)
#### Способности:
##### Выстрелы 
Ведьма стреляет стрелами на откидывание и уроном.
##### Подкидывание 
Ведьма подкидывает игроков в радиусе и резко бросает их на землю.
##### Призыв друидов
Ведьма призывает вокруг друидов.
### Восстание
![enter image description here](https://github.com/Lairon1/MSCClans-wiki/blob/main/images/Insurrection.png) 
Зомби вылезают из под земли в определенной точке у раках с хорошими мечами.
## Placeholders
%clan_tag% - вернет тег клана с цветовым кодом.

%clan_id% - вернет тег клана без цветового кода.

%clan_participant% - вернет роль в клане.(Глава, модератор, участник)

%clan_exp% - вернет опыт клана.

%clan_level% - вернет уровень клана.

## Конфиг
```no-highlight
Preffix: "&9&lMSCClans 7»"

Messages:
  COMMANDS:
  - "&7Неверное использование команды &9/clan&7."
  - "&7Доступные &9команды&7:"
  - "&9/clan create <ТЕГ> &7- Создать клан."
  
  #MISC
  IS_CREATED: "&7Клан с таким &9ID &7уже существует!"
  NO_MONEY: "&7У вас недостаточно денег на балансе! вам нужно &9%money_amount%&7$."
  NO_PERM: "&7У вас нет прав на это!"
  DONE_CREATION: "&7Вы успешно создали клан &9%clan_id%&7."
  CANT_CREATE: "&7Вы не можете создать &9клан, &7так как уже состоите в другом." 
  RELOAD_CONFIG: "&7Конфиг успешно перезагружен."
  NOT_MEMBER: "&7Вы не состоите в &9клане&7."   
  DISBAND: "&7Вы успешно &cраспустили &7свой клан."
  CREATE_ERR: "&9ID клана &7которое вы ввели не соответствует патерну."
  BY_SELF: "&7А себя только &9плеткой&7 по попке."  
  NO_ONLINE: "&7Этот игрок не &9онлайн&7."  
  ALREADY_IN: "&7Этот &9игрок уже состоит в клане."    
  WELCOME_MEMBER: "&7Вы успешно вступили в клан &9%clanid%&7."
  GIVE_DONE: "&7Вы успешно &7передали свой клан."
  DO_IT: "&7Вы действительно хотите сделать это?"
  NOT_CREATE: "&7Этот клан еще не &9создан&7." 
  
  #ONLY
  ONLY_OWNER: "&7Это может делать только &9глава&7 клана."   
  ONLY_MODERATOR: "&7Это могут делать только &9Модероторы&7 и выше."
  ONLY_PLAYER: "&7Эту команду может использовать только игрок."
  
  #PROMOTE
  PROMORE_ERR: "&7Игрок уже является &9Модератором&7."
  PROMOTE_DONE: "&7Теперь игрок &9%promote_player%&7 Модератор."
  
  #COLOR
  COLOR_DONE: "&7Вы успешно сменили &9цвет&7 клана."
  COLOR_ERR: "&7Данный &9цвет &7клана не поддерживается."
  
  #KICK
  KICK_ERR: "&7Вы не можете &9кикнуть&7 этого игрока."
  KICK_DONE: "&7Вы успешно кикнули &9%kick_name%&7 из клана."
  
  #LEVEL/EXP
  LEVEL_NOT_ALLOW: "&7Ваш &9уровень&7 клана пока не позволяет использовать это. &9Прокачайте&7 его и эта функция станет доступна."
  EXP_BAR: "+&9%exp% &7очков клана"
  
  #LEAVE
  LEAVE_DONE: "&7Вы успешно &9вышли&7 из клана."
  LEAVE_ERR: "&7Вы не можете &9выйти&7 из клана, так как вы глава клана. Вы можете только распустить клан (&9/clan disband&7) или передать(&9/clan give <player_name>&7)."
  
  #DEPOSIT/TAKE
  DEPOSIT_ERR: "&7У вас нету таких денег."
  DEPOSIT_DONE: "&7Вы успешно перевели &9монеты&7 на баланс клана."
  TAKE_DONE: "&7Вы успешно забрали &9монеты&7 с баланса клана."
  
  #PVP
  PVP_TRUE: "&7Вы успешно &9включили&7 пвп в клане."
  PVP_FALSE: "&7Вы успешно &9выключили&7 пвп в клане."
  
  #HOME
  HOME_TP_DONE: "Вы телепортированы на базу клана &9%clanid%&7."
  HOME_PRIVATE: "&7У этого клана &9приватная&7 клановая база, либо она еще не &9создана&7."
  HOME_ERR: "&7У вас еще не &9установлена&7 клановая база."
  HOME_OPEN: "&7Вы успешно &9открыли&7 клановую базу."
  HOME_CLOSE: "&7Вы успешно &9закрыли&7 клановую базу."
  HOME_DELETE: "&7Вы успешно &9удалили&7 клановую базу."
  HOME_SET_DONE: "&7Вы успешно &9установили&7 клан базу."
  
  #WelcomeMSG
  WELCOME_REMOVE: "&7Вы &9удалили&7 клановое сообщение."
  WELCOME_SET: "&7Вы &9установили&7 сообщение клана."
  
  #Invite
  INVITE_DONT: "&7У вас нет &9приглашения&7 в этот клан."
  INVITE_ACCEPT_ERR: "&7Вы уже состоите в &9клане&7."
  INVITE: "&7Игрок &9%inviter_name% &7пригласил вас в клан &9%clanid%&7 \nДействия:"
  INVITE_AGAIN: "&7У данного игрока уже есть приглашение в ваш &9клан&7."
  INVITE_DONE: "&7Вы успешно пригласили игрока &9%name%&7 в клан."
  
  #Alliance
  ALLIANCE_OFFLINE: "&7Глава клана которому вы пытаетесь предложить союз &9не онлайн&7."
  ALLIANCE_INVITE_DONE: "Вы успешно предложили союз клану %clantag%."
  ALLIANCE_SOLUTION: "&7Клан %clantag% предлагает вам &9союз&7. Действия:"
  ALLIANCE_DONE_INVITER: "&7Клан %clantag% &9одобрил&7 запрос о союзе."
  ALLIANCE_DONE_INVITE: "&7Теперь вы в &9союзе&7 с кланом %clantag%"
  ALLIANCE_ERR: "&7У вас нет &9запроса&7 на союз от этого клана."
  ALLIANCE_INVITE_AGAIN: "&7Вы уже &9отплавили&7 запрос на союз этому клану."
  ALLIANCE_REMOVE: "&7Вы &9расторгли&7 альянс с кланом %clantag%."
Buttons:
  Accept: "&7[&aПОДТВЕРДИТЬ&7]"
Holograms:
  #Раз во сколько тиков будет обновлятся галограмма.(Не ставите слишком маленькое число сервер может зависнуть.)
  Update: 200
  Bank:
    Title: "Топ &9кланов&f по балансу."
    Style: "&7[%clanTag%&7] &9%bank%"
  Members:
    Title: "Топ &9кланов&f по кол-ву участников."
    Style: "&7[%clanTag%&7] &9%members%"
  Level:
    Title: "Топ &9кланов&f по уровню."
    Style: "&7[%clanTag%&7] &9%level%"
  Exp:
    Title: "Топ &9кланов&f по опыту."
    Style: "&7[%clanTag%&7] &9%exp%"
Settings:  
  #Патерн которому должны СООТВЕ́ТСТВОВАТЬ все ID кланов
  #Не трогай если не знаешь как работают регулярные выражения
  PATTERN: "^[A-Za-z][A-Za-z0-9]{3}$"         
  #Сколько нужно денег для создания клана(Только целое число INT)
  CREATE_MONEY: 150000
  #Сколько нужно монет на изменение цвета клана (Только целое число INT)
  COLOR_MONEY: 15000
  #Сколько нужно монет чтобы поставить клановую базу(Только целое число INT)
  NOME_MONEY: 15000
  CHAT: "&7[&9Клан-чат&7] &7%player_name%: %message%"
  Events:
    #Если false ивенты работать не будут
    ENABLE: true
    #Какое минимальное количество кланов должно быть в сети чтобы мог начатся ивент
    MIN_CLANS: 0
    #В каком радиусе от 0 координаты возможен спавн ивента. 
    RADIUS: 1
    #В каком мире будут спавнится ивенты.
    WORLD: "world"
    #Через сколько мс начнется ивент после его обьявления
    TIME: 1000
    #Если игрок пишет /event когда событие еще не началось
    NOT_START: "&7Клановое событие еще не началось."
    #Если игрок пишет /event когда событие скоро начнется
    START_TIMER: "&7Клановое событие %event%&7 начнется через &9%time%&7.\nКординаты:\n&7X: &9%x%\n&7Y: &9%y%\n&7Z: &9%z%"
    #Если игрок пишет /event когда событие уже началось
    START: "&7Клановое событие %event%&7 уже началось.\nКординаты:\n&7X: &9%x%\n&7Y: &9%y%\n&7Z: &9%z%"
    #Настройка ивента "Красный демон"
    RedDemon:
      #Если false этот ивент работать не будет.
      Enable: true
      #Оповещение о начале ивента
      StartTimerMSG: "&7Клановое событие &0Красный демон&7 начнется через 5 минут! \n/event - подробная информация."
      #Имя босса
      Name: "&0Красный демон"
      #Сколько у него хп максимальное число 2048
      Health: 2048
      #Сообщение о начале ивента
      Broadcast: "&7Клановое событие &0Красный демон&7 началось! \n &c/event - подробная информация."
      #После какого значения HP Будет включатся режим ярости
      RageHP: 300
      #Тайтл который показывается при переходе демона в ярость
      RageTitle: "Демон в ярости! Бегите"
      #Какое время демон будет находится в ярости. В мс.
      RageTime: 30000
      #Какой урон будет наносить демон в ярости
      RageDamage: 30
      #Сколько будет наносится урона по радиусу
      SplashDamage: 23
      #Урон ускорением
      Acceleration: 25
      #Имя друидов
      DruidName: "&cДруид"
      #Текст боссБара
      BossBar: "&0Красный демон&7: [&c%nowhp%&7/&c%maxhp%&7hp] Лидер: %clan%"
      #Текст босбара при победе
      BossBarWin: "&aКрасный демон побежден! Победитель: %clan%"
      #Хп друидов
      DruidHP: 1
      #Что выводить в ActionBar при ударе.
      ActionBar: "&cНанесен урон вашим кланом: &c%damage%"
      #Сообщение о окончании ивента
      BroadcastEventCansel: "&7Победу в ивенте &cКрасный демон&7 одерживает клан %clan% \n&7Награда: &910000&7 ед. опыта"
      #Какое количество опыта получит клан если выйграет
      Prize: 10000
    #Настройка ивента "Ведьма"
    Magician:
      #Если false этот ивент работать не будет.
      Enable: true
      #Оповещение о начале ивента
      StartTimerMSG: "&7Клановое событие &5Ведьма&7 начнется через 5 минут! \n/event - подробная информация."
      #Имя босса
      Name: "&5Ведьма"
      #Сколько у него хп максимальное число 2048
      Health: 2048
      #Сообщение о начале ивента
      Broadcast: "&7Клановое событие &5Ведьма&7 началось! \n &c/event - подробная информация."
      #Какой урон будет наносить стрелла
      ArrowDamage: 3
      #С какой силой будут одталкивать стрелы
      ArrowKnockback: 2
      #Урон который будет наносится при подкидывании игрока в воздух
      Acceleration: 25
      #Имя друидов
      DruidName: "&5Друид"
      #Текст боссБара
      BossBar: "&5Ведьма&7: [&c%nowhp%&7/&c%maxhp%&7hp] Лидер: %clan%"
      #Текст босбара при победе
      BossBarWin: "&aВедьма побеждена! Победитель: %clan%"
      #Хп друидов
      DruidHP: 1
      #Что выводить в ActionBar при ударе.
      ActionBar: "&cНанесен урон вашим кланом: &c%damage%"
      #Сообщение о окончании ивента
      BroadcastEventCansel: "&7Победу в ивенте &9Ведьма&7 одерживает клан %clan% \n&7Награда: &910000&7 ед. опыта"
      #Какое количество опыта получит клан если выйграет
      Prize: 10000
    #Настройка ивента "Восстание"
    Insurrection:
      #Если false этот ивент работать не будет.
      Enable: false
      #Оповещение о начале ивента
      StartTimerMSG: "&7Клановое событие &cВосстание&7 начнется через 5 минут! \n/event - подробная информация."
      #Имя события
      EventName: "&cВосстание&7"
      #Имя зомби
      Name: "&cМертвец"
      #Максимально количество зомби
      QuantityMax: 1000
      #Количество зомби которое может существовать одновременно
      QuantityNow: 10
      #Сколько у зомби будет хп
      Health: 30
      #Сообщение о начале ивента
      Broadcast: "&7Клановое событие &сВосстание&7 началось! \n &c/event - подробная информация."
      #На какую остроту бутет мечь у зомби
      Damage: 20
      #Скорость зомби
      Speed: 1
      #Текст боссБара
      BossBar: "&cВосстание&7: [&c%nowZ%&7/&c%maxZ%&7] Лидер: %clan%"
      #Текст босбара при победе
      BossBarWin: "&aВосстание обезврежено! Победитель: %clan%"
      #Что выводить в ActionBar при ударе.
      ActionBar: "&cУбито зомби вашим кланом: &c%zomb%"
      #Сообщение о окончании ивента
      BroadcastEventCansel: "&7Победу в ивенте &cВосстание&7 одерживает клан %clan% \n&7Награда: &910000&7 ед. опыта"
      #Какое количество опыта получит клан если выйграет
      Prize: 10000
  #Уровни клана
  Levels:
    #Номер уровня. первый уровень идет изначально и получить его снова нельзя. используйте кго как шаблон и пример.
    1:
      #Сколько нужно EXP клана чтобы перейти на следующий уровень.
      NextLevelEXP: 500
      #Максимальное количество участников клана(Всех в месте "Глава,модераторы,участники")
      MaxMembers: 5
      #Максимальное количество модераторов клана.
      MaxModerators: 1
      #Сколько выдать монет при переходе на этот уровень
      BankGiveMoney: 0
      #Может ли клан создать клановую базу.
      CanCreateCH: false
      #Может ли клан поменять цвет клана.
      ClanColor: false
      #Сообщение для клана после перехода на этот уровень.
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Ваш клан достиг &91-вого&7 уровня."
      - "&7Теперь у вас:"
      - "&95 &7слотов для участников."
      - "&91 &7слот для модератора."
      - "&9██████████████████████████"
    2:
      NextLevelEXP: 1000
      MaxMembers: 10
      MaxModerators: 2
      BankGiveMoney: 10000
      CanCreateCH: false
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Ваш клан достиг &92-го&7 уровня."
      - "&7Теперь у вас:"
      - "&910 &7слотов для участников."
      - "&92 &10слотов для модераторов."
      - "&9+ 10000$ &7в банк клана."
      - "&9██████████████████████████"
    3:
      NextLevelEXP: 2000
      MaxMembers: 10
      MaxModerators: 3
      BankGiveMoney: 0
      CanCreateCH: false
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Ваш клан достиг &93-го&7 уровня."
      - "&9██████████████████████████"
    4:
      NextLevelEXP: 3800
      MaxMembers: 15
      MaxModerators: 3
      BankGiveMoney: 15000
      CanCreateCH: false
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Ваш клан достиг &94-го&7 уровня."
      - "&7Теперь у вас:"
      - "&915 &7слотов для участников."
      - "&9+ 15000$ &7в банк клана."
      - "&9██████████████████████████"
    5:
      NextLevelEXP: 5000
      MaxMembers: 15
      MaxModerators: 5
      BankGiveMoney: 0
      CanCreateCH: false
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &95-го&7 уровня."
      - "&7Теперь у вас:"
      - "&95 &7слотов для модераторов"
      - "&9██████████████████████████"
    6:
      NextLevelEXP: 6000
      MaxMembers: 20
      MaxModerators: 5
      BankGiveMoney: 20000
      CanCreateCH: false
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &96-го&7 уровня."
      - "&7Теперь у вас:"
      - "&920 &7слотов для участников."
      - "&9+ 20000$ &7в банк клана."
      - "&9██████████████████████████"
    7:
      NextLevelEXP: 7500
      MaxMembers: 20
      MaxModerators: 7
      BankGiveMoney: 20000
      CanCreateCH: false
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &97-го&7 уровня."
      - "&7Теперь у вас:"
      - "&97 &7слотов для модераторов."
      - "&9██████████████████████████"      
    8:
      NextLevelEXP: 9000
      MaxMembers: 25
      MaxModerators: 7
      BankGiveMoney: 25000
      CanCreateCH: false
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &98-го&7 уровня."
      - "&7Теперь у вас:"
      - "&925 &7слотов для участников."
      - "&9+ 25000$ &7в банк клана."
      - "&9██████████████████████████" 
    9:
      NextLevelEXP: 10000
      MaxMembers: 25
      MaxModerators: 7
      BankGiveMoney: 0
      CanCreateCH: false
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Ваш клан достиг &99-го&7 уровня."
      - "&9██████████████████████████" 
    10:
      NextLevelEXP: 11000
      MaxMembers: 30
      MaxModerators: 9
      BankGiveMoney: 30000
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &910-го&7 уровня."
      - "&7Теперь у вас:"
      - "&930 &7слотов для участников"
      - "&99 &7слотов для модераторов"
      - "&9+ 30000$ &7в банк клана."
      - "&7Теперь глава может установить &9клановую &7базу."
      - "&9█████████████████████████      
    11:
      NextLevelEXP: 12500
      MaxMembers: 30
      MaxModerators: 10
      BankGiveMoney: 0
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Ваш клан достиг &911-го&7 уровня."
      - "&7Теперь у вас:"
      - "&910 &7слотов для модераторов"
      - "&9██████████████████████████"
    12:
      NextLevelEXP: 13000
      MaxMembers: 30
      MaxModerators: 10
      BankGiveMoney: 35000
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &912-го&7 уровня."
      - "&7Теперь у вас:"
      - "&9+ 35000$ &7в банк клана."      
      - "&9██████████████████████████"     
    13:
      NextLevelEXP: 14500
      MaxMembers: 35
      MaxModerators: 10
      BankGiveMoney: 0
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &913-го&7 уровня."
      - "&7Теперь у вас:"
      - "&930 &7слотов для участников"   
      - "&9██████████████████████████"  
    14:
      NextLevelEXP: 16500
      MaxMembers: 35
      MaxModerators: 12
      BankGiveMoney: 0
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &914-го&7 уровня."
      - "&9██████████████████████████"          
    15:
      NextLevelEXP: 17000
      MaxMembers: 35
      MaxModerators: 12
      BankGiveMoney: 0
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &915-го&7 уровня."
      - "&7Теперь у вас:"
      - "&9+ 35000$ &7в банк клана."        
      - "&9██████████████████████████"     
    16:
      NextLevelEXP: 18000
      MaxMembers: 35
      MaxModerators: 14
      BankGiveMoney: 0
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &916-го&7 уровня."
      - "&7Теперь у вас:"
      - "&914 &7слотов для модераторов"  
      - "&9██████████████████████████" 
    17:
      NextLevelEXP: 19500
      MaxMembers: 40
      MaxModerators: 12
      BankGiveMoney: 0
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &917-го&7 уровня."
      - "&7Теперь у вас:"
      - "&940 &7слотов для участников"    
      - "&9██████████████████████████"
    18:
      NextLevelEXP: 20000
      MaxMembers: 40
      MaxModerators: 12
      BankGiveMoney: 45000
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &918-го&7 уровня."
      - "&7Теперь у вас:"
      - "&9+ 45000$ &7в банк клана."        
      - "&9██████████████████████████"        
    19:
      NextLevelEXP: 22500
      MaxMembers: 40
      MaxModerators: 12
      BankGiveMoney: 0
      CanCreateCH: true
      ClanColor: false
      Message:
      - "&9██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &919-го&7 уровня."
      - "&9██████████████████████████"             
    20:
      NextLevelEXP: 25000
      MaxMembers: 50
      MaxModerators: 15
      BankGiveMoney: 50000
      CanCreateCH: true
      ClanColor: true
      Message:
      - "&d██████████████████████████"
      - "&7Поздравляю! Вашь клан достиг &d20-го&7 уровня."
      - "&7Теперь у вас:"
      - "&950 &7слотов для участников"
      - "&d15 &7слотов для модераторов"
      - "&d+ 50000$ &7в банк клана."
      - "&7Теперь глава может поставить &dцвет &7клана."
      - "&d██████████████████████████"
  #Сколько будет падать с каждого моба EXP (default будет применятся если в списке животного нет.)  
  MobKillEXP:
    default:
      minEXP: 20
      maxEXP: 40
    COW:
      minEXP: 5
      maxEXP: 15
    PIG:
      minEXP: 5
      maxEXP: 15
    Chicken:
      minEXP: 10
      maxEXP: 20
    Sheep:
      minEXP: 5
      maxEXP: 15
    Wolf:
      minEXP: 15
      maxEXP: 30
    Horse:
      minEXP: 5
      maxEXP: 15     
    Ocelot:
      minEXP: 20
      maxEXP: 40
    Mooshroom:   
      minEXP: 20
      maxEXP: 40
    Skeleton: 
      minEXP: 5
      maxEXP: 15
    Zombie: 
      minEXP: 5
      maxEXP: 15    
    spider: 
      minEXP: 5
      maxEXP: 15
    cave_spider: 
      minEXP: 7
      maxEXP: 15
    ghast: 
      minEXP: 7
      maxEXP: 15
    wither_Skeleton: 
      minEXP: 7
      maxEXP: 15  
    Blaze: 
      minEXP: 7
      maxEXP: 15
    magma_cube: 
      minEXP: 7
      maxEXP: 15
    Wither: 
      minEXP: 100
      maxEXP: 150
    Rabbit:  
      minEXP: 3
      maxEXP: 5
    Creeper: 
      minEXP: 7
      maxEXP: 15
    Enderman: 
      minEXP: 10
      maxEXP: 15
    zombified_piglin:  
      minEXP: 7
      maxEXP: 15
    ender_dragon: 
      minEXP: 200
      maxEXP: 300
    golem: 
      minEXP: 15
      maxEXP: 30
    snow_golem: 
      minEXP: 7
      maxEXP: 10
    Slime: 
      minEXP: 7
      maxEXP: 15      
    Witch:   
      minEXP: 10
      maxEXP: 15      
    Guardian:
      minEXP: 20
      maxEXP: 30   
    Squid:
      minEXP: 7
      maxEXP: 15   
      
```
