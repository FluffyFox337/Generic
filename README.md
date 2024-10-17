# Generic+++ RU
Генерация WARP и WARP+ профилей

Суть работы такова: 
* Создайте где нибудь папку, закиньте туда генератор Generic+++.exe и Generic.conf (по желанию)
* При запуске проверяется проверяется наличие интернета - пингуется google.com. Дальше проверяется наличие в папке утилиты wgcf.exe (Если ее нет скачивается.)
* Дальше проверяется наличие C:\Program Files\AmneziaWG\amneziawg.exe и Generic.conf, от наличия\отсутствия Generic.conf различное поведение программы.
  
Generic.conf - (упакован в zip) это профиль. Нужен тем у кого нет вообще ни одного профиля и VPN поднять нечем. 
У кого не работает редактируем Endpoint либо подключаем временно любой работающий VPN, ибо без VPN сгенерить профили не получится!

Два варианта работы:
1. (Без использования Generic.conf = в папке его нет)
   * Подключаем рабочий VPN (не в браузере) 
   * запускаем генератор выскакивает окошко в котором можно указать свой Endpoint либо нажать ОК будет использован вариант (по умолчанию engage.cloudflareclient.com:2408)
   * генерируются 5 аккаунтов, (один из которых переименовывается в Generic.conf, чтобы был свой, а не общественный) со значением Endpoint который выбрали и тремя случайно сгенерированными параметрами Jc Jmin Jmax.
3. (С использованием Generic.conf = в папке он ЕСТЬ) 
   * Если генератор обнаруживает Generic.conf, то пытается поднять тоннель с этим Generic.conf (любые другие VPN должны быть отключены иначе туннель не поднимется), 
   * дальше проверяет интернет, если все ок генерирует 5 конфигураций.
	(Можно закинуть точно работающий профиль в папку, переименовать в Generic.conf и сгенерить профили/конфигурации)

Добавлена возможность генерации лицензионных профилей, ключ лицензии должен быть в буфере. Ключ можно сгенерировать например здесь: [ https://t.me/warpkeygenbot ]

В связи с тем, что у многих клиент не заводится на адресе 162.159.193.1:2408 установленном по умолчанию в генераторе, генератор был переписан. Теперь адрес остается по умолчанию (Endpoint = engage.cloudflareclient.com:2408) если в окне для ввода конечной точки (Endpoint) не прописан свой. Добавлен запрос прав Администратора. Изменено имя на Generic+++. Изменена версия. Изменен Generic.conf.


# Generic+++ EN
Generate WARP/WARP+ profiles

The essence of the work is: 
* Create a folder somewhere, drop in the generator Generic+++. exe and Generic.conf (optional)
* When starting up, the internet is checked - google.com is pinged. Next check if the folder has wgcf.exe (If it does not download.)
* Next, the presence of C:\Program Files\AmneziaWG\amneziawg.exe and Generic.conf is checked, if there is no Generic.conf different behavior of the program.
  
Generic.conf - (packed in zip) is a profile. It needs someone who doesn’t have any profiles at all and VPN doesn’t have anything to raise. 
If you do not work edit the Endpoint or connect any temporarily working VPN, because without VPN to generate profiles will not work!

Two options for work:
1. (Without using Generic.conf = the folder is empty)
   By connecting the working VPN (not in the browser) running the generator pops up a window where you can specify your Endpoint or press OK will be used default option 162.159.193.1:2408 - generated 5 accounts, (one of which 
   is renamed to Generic.conf, so it’s its own, not a public one) with the Endpoint value you chose and three randomly generated Jc Jmin Jmax parameters.
3. (Generic.conf in folder) If the generator detects Generic.conf
    Tries to raise the tunnel with this Generic.conf (any other WPS must be disabled otherwise the tunnel will not rise), then checks the internet if all ok generates 5 configurations. (You can put a precisely working profile in the folder, 
    rename to Generic.conf and generate profiles (configuration))
5. Added the ability to generate license profiles, license key must be in buffer. Key can be generated for example here: [ https://t. me/warpkeygenbot ]

Due to the fact that many customers do not start at the address 162.159.193.1:2408 set by default in the generator, the generator was rewritten. The address now remains the default (Endpoint = engage.cloudflareclient.com:2408) if the input window for the endpoint (Endpoint) is not typed in. Added Administrator rights request. Changed name to Generic+++. Changed version. Changed Generic.conf.
