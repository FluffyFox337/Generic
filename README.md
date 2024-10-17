# Generic+++
Генерация WARP и WARP+ профилей

Суть работы такова: 
* Создайте где нибудь папку, закиньте туда генератор Generic+++.exe и Generic.conf (по желанию)
* При запуске проверяется проверяется наличие интернета - пингуется google.com. Дальше проверяется наличие в папке утилиты wgcf.exe (Если ее нет скачивается.)
* Дальше проверяется наличие C:\Program Files\AmneziaWG\amneziawg.exe и Generic.conf, от наличия\отсутствия Generic.conf различное поведение программы.
  
Generic.conf - (упакован в zip) это профиль. Нужен тем у кого нет вообще ни одного профиля и ВПН поднять нечем. 
У кого не работает редактируем Endpoint либо подключаем временно любой работающий ВПН, ибо без ВПН сгенерить профили не получится!

Два варианта работы:
1. (Без использования Generic.conf = в папке его нет)
   Подключаем рабочий ВПН (не в браузере) запускаем генератор выскакивает окошко в котором можно указать свой Endpoint либо нажать ОК будет использован вариант по умолчанию 162.159.193.1:2408 - генерируются 5 аккаунтов, (один из которых 
   переименовывается в Generic.conf, чтобы был свой, а не общественный) со значением Endpoint который выбрали и тремя случайно сгенерированными параметрами Jc Jmin Jmax.
3. (Generic.conf в папке) Если генератор обнаруживает Generic.conf
    то пытается поднять тоннель с этим Generic.conf (любые другие ВПН должны быть отключены иначе туннель не поднимется), дальше проверяет интернет, если все ок генерирует 5 конфигураций. (Можно закинуть точно работающий профиль в папку, 
    переименовать в Generic.conf и сгенерить профили (конфигурации))
5. Добавлена возможность генерации лицензионных профилей, ключ лицензии должен быть в буфере. Ключ можно сгенерировать например здесь: [ https://t.me/warpkeygenbot ]

В связи с тем, что у многих клиент не заводится на адресе 162.159.193.1:2408 установленном по умолчанию в генераторе, генератор был переписан. Теперь адрес остается по умолчанию (Endpoint = engage.cloudflareclient.com:2408) если в окне для ввода конечной точки (Endpoint) не прописан свой. Добавлен запрос прав Администратора. Изменено имя на Generic+++. Изменена версия. Изменен Generic.conf.



# Generic+++
Generate WARP profile

The essence of the work is as follows: Create a folder somewhere, throw there generator Generic+++. exe and Generic.conf (if desired)
When running, check for internet presence - pinged google.com. Next check for wgcf.exe utility in folder.
If it is not available.
Next, check for C: Program Files AmneziaWG amneziawg.exe and Generic.conf, if there is no Generic.conf different behavior of the program.
Generic.conf - (packed in zip, because it’s not possible to attach otherwise) is a profile. Generic.conf is needed by those who don’t have any profiles at all and PHP doesn’t have anything to raise. If you don’t have a working Endpoint edit or try the options written several posts above, because without WPS to generate a profile it will not work!

Two options for work:
1. (without using Generic.conf = in the folder it is not) We connect working VPM (not in browser) start generator pop-up window in which you can specify your Endpoint or press OK will be used default option 162.159.193.1:2408 - generated 5 accounts,  (one of which is renamed to Generic.conf to be its own, not public) with the endpoint value chosen and three randomly generated JC parameters Jmin Jmax.
2. (Generic.conf in folder) If the generator detects Generic.conf then it tries to raise the tunnel with this Generic.conf (any other WPS must be disabled otherwise the tunnel will not rise), further checks the internet if all of them generate 5 configurations.
3. (You can put an exactly working profile in a folder, rename it to Generic.conf and generate profiles (configuration))
4. Added the ability to generate license profiles, license key must be in buffer. Key can be generated for example here:
5. https://t.me/warpkeygenbot

Due to the fact that many customers do not start at the address 162.159.193.1:2408 set by default in the generator, the generator was rewritten. The address now remains the default (Endpoint = engage.cloudflareclient.com:2408) if the input window for the endpoint (Endpoint) is not typed in. Added Administrator rights request. Changed name to Generic+++. Changed version. Changed Generic.conf.
