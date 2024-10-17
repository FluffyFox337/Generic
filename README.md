# Generic+++ RU
Генерация WARP и WARP+ профилей

Суть работы такова: 
* Создайте где нибудь папку, закиньте туда генератор Generic+++.exe и Generic.conf (по желанию)
* При запуске проверяется проверяется наличие интернета - пингуется google.com. Дальше проверяется наличие в папке утилиты wgcf.exe (Если ее нет скачивается.)
* Дальше проверяется наличие C:\Program Files\AmneziaWG\amneziawg.exe и Generic.conf, от наличия\отсутствия Generic.conf различное поведение программы.
  
Generic.conf - (упакован в zip) это профиль. Нужен тем у кого нет вообще ни одного профиля и VPN поднять нечем. 
У кого не работает редактируем Endpoint либо подключаем временно любой работающий VPN, ибо без VPN сгенерить профили не получится!

Два варианта работы:
1. Без использования Generic.conf = в папке его нет
   * Подключаем рабочий VPN (не в браузере).
   * Запускаем генератор выскакивает окошко в котором можно указать свой Endpoint либо нажать ОК будет использован вариант (по умолчанию engage.cloudflareclient.com:2408).
   * Генерируются 5 аккаунтов, (один из которых переименовывается в Generic.conf, чтобы был свой, а не общественный) со значением Endpoint который выбрали и тремя случайно сгенерированными параметрами Jc Jmin Jmax.
3. С использованием Generic.conf = в папке он ЕСТЬ
   * Если генератор обнаруживает Generic.conf, то пытается поднять тоннель с этим Generic.conf (любые другие VPN должны быть отключены иначе туннель не поднимется).
   * Дальше проверяет интернет, если все ок генерирует 5 конфигураций.
	(Можно закинуть точно работающий профиль в папку, переименовать в Generic.conf и сгенерить профили/конфигурации)

- Добавлена возможность генерации WARP+ профилей, ключ лицензии должен быть в буфере. 
  Ключ можно сгенерировать например здесь: [ https://t.me/warpkeygenbot ]

- В связи с тем, что у многих клиент не заводится на адресе 162.159.193.1:2408 установленном по умолчанию в генераторе, генератор был переписан. Теперь адрес остается по умолчанию (Endpoint = engage.cloudflareclient.com:2408) если в окне для ввода конечной точки (Endpoint) не прописан свой. Добавлен запрос прав Администратора. Изменено имя на Generic+++. Изменена версия. Изменен Generic.conf.


# Generic+++ EN
Generate WARP/WARP+ profiles

The essence of the work is: 
* Create a folder somewhere, drop in the generator Generic+++. exe and Generic.conf (optional).
* When starting up, the internet is checked - google.com is pinged. Next check if the folder has wgcf.exe (If it does not download).
* Next, the presence of C:\Program Files\AmneziaWG\amneziawg.exe and Generic.conf is checked, if there is no Generic.conf different behavior of the program.
  
Generic.conf - (packed in zip) is a profile. It needs someone who doesn’t have any profiles and the VPN has nothing to raise. 
If you don’t have a working Endpoint, edit it or connect any VPN temporarily, because without a VPN you can’t get profiles!

Two options for work:
1. Without using Generic.conf = the folder does not contain it
   * Connect to a working VPN (not in a browser).
   * When running the generator pops up a window in which you can specify your Endpoint or press OK option will be used (default is engage.cloudflareclient.com:2408).
   * Generate 5 accounts (one of which is renamed to Generic.conf, so that it is yours and not public) with the Endpoint value you have chosen and three randomly generated parameters Jc Jmin Jmax.
3. Using Generic.conf = in the folder it IS
   * If the generator detects Generic.conf, it tries to raise the tunnel with this Generic.conf (any other VPN must be disabled otherwise the tunnel will not rise)
   * Next checks if all ok generates 5 configurations.
	(You can put a working profile in a folder, rename it to Generic.conf and generate profiles/configurations)

- Added the ability to generate WARP+ profiles, license key must be in buffer. 
  Key can be generated for example here: [https://t.me/warpkeygenbot]

- Due to the fact that many customers do not start at the address 162.159.193.1:2408 set by default in the generator, the generator was rewritten. The address now remains the default (Endpoint = engage.cloudflareclient.com:2408) if the input window for the endpoint (Endpoint) is not typed in. Added Administrator rights request. Changed name to Generic+++. Changed version. Changed Generic.conf.

# FAQ RU
1. Что такое Jc Jmin Lmax ?
   * Jc = junk_packet_countJc (Junk packet count) — количество пакетов со случайными данными, отправленных до начала сеанса.
   * JMin = junk_packet_min_sizeJMin (Junk packet minimum size) - минимальный размер пакета для Junk packet.
     То есть все случайно сгенерированные пакеты будут иметь размер не меньше Jmin.JMax = junk_packet_max_sizeJMax (максимальный размер мусорного пакета) — максимальный размер мусорных пакетов.
2. Какие значения указывать для Jc Jmin Lmax?
   * Параметры J вы можете изменять как вам захочется, но Jc должно быть от 1 до 128. (много не пишите, хватит 3-10).
   * Jmin не должно превышать Jmax.
   * Jmax должно быть не больше 1280.
   * Пример настройки Jc Jmin Lmax:
      * Jc = 3
      * Jmin = 10
      * Jmax = 50

AmneziaWG (AmneziaWireGuard) — это форк обычного WireGuard-Go с добавлением функций обхода блокировок и снижения вероятности обнаружения протоколов. Одной из ключевых особенностей AmneziaWG является обратная совместимость с WireGuard. Это означает, что при использовании AmneziaWG, если в конфигурации не указаны специальные параметры для "обфускации" протоколов, он будет действовать как стандартный WireGuard. В практическом применении это дает обход существующих блокировок по IP и ТСПУ — технические средства противодействия угрозам (что, конечно, не совсем законно), в потребительском - рабочий Youtube и просмотр сайтов запрещенных РКН (что тоже не очень законно). Конфигурации с дополнительными параметрами в классическом WireGuard работать не будут.

Конечно ни о какой полноценной "обфускации" тут речи идти не может и механизм заложенный в этом клиенте не уникален, современные приложения для VPN давно используют метод "мусорных пакетов". Сам протокол WireGuard внутри туннеля шифруется, но на этапе "рукопожатия" легко детектируется системами DPI(ТСПУ) - Deep Packet Inspection — технология проверки сетевых пакетов по их содержимому с целью регулирования и фильтрации трафика, а также накопления статистических данных.

AmneziaWG перед созданием защищенного туннеля посылает несколько безобидных пакетов (Jc, Jmin, Jmax) число и размер которых случайный (настраивается в профиле (конфигурации профиля)), тем самым заставляя систему DPI думать, что это обычный трафик. Конечно это не панацея и были уже случаи когда просто блокировались все неопознанные протоколы, но в глобальном масштабе это 'сейчас' едва ли применимо.
Однако все меняется очень быстро и дать гарантии, что ТСПУ не научат, каким то образом, выявлять эти мусорные пакеты никто не может, благо таких клиентов становится все больше и они используют не только протокол WireGuard, да и рандомизация этих пакетов практически сводит на "нет" возможность классификации. С теорией покончили.

# FAQ EN
1. What is Jc Jmin Lmax ?
   * Jc = junk_packet_countJc (Junk packet count) — the number of packets with random data sent before the session starts.
   * JMin = junk_packet_min_sizeJMin (Junk packet minimum size) - The minimum package size for a Junk packet.
     That is, all randomly generated packets will have a size of at least Jmin.JMax = junk_packet_max_sizeJMax (maximum size of the garbage packet) - the maximum size of the garbage packets.
2. What values to specify for Jc Jmin Lmax?
   * Parameters J you can change as you like, but Jc should be from 1 to 128. (don’t write much, 3-10 is enough).
   * Jmin must not exceed Jmax.
   * Jmax should be no more than 1280.
   * Example of setting up a JC Jmin Lmax:
      * Jc = 3
      * Jmin = 10
      * Jmax = 50

AmneziaWG (AmneziaWireGuard) is a forking of the usual WireGuard-Go, with the addition of blocking and protocol detection. One of the key features of AmneziaWG is reverse compatibility with WireGuard. This means that when using AmneziaWG, if no special configuration is specified for "bypass" protocols, it will act as standard WireGuard. In practical application, this gives bypass of existing blocks on IP and TSPU - technical means to counter threats (which, of course, is not quite legal), in consumer - working Youtube and viewing sites banned by PKN (which also not very legal). Configurations with additional parameters in classic WireGuard will not work.

Of course, no full "Ausausausesing" can be talked about here and the mechanism built in this client is not unique, modern applications for VPN have long used the method of "junk packets". The WireGuard protocol inside the tunnel is encrypted, but in the "handshake" phase it is easily detected by DPI(TSPU) systems - Deep Packet Inspection - a technology to check network packets for their content in order to regulate and filter traffic and store statistical data.

AmneziaWG before creating a protected tunnel sends several harmless packets (Jc, Jmin, Jmax) whose number and size are random (configured in the profile (profile configurations)), thus making the DPI system think that it is normal traffic. Of course this is not a panacea and there have been cases where all unidentified protocols are simply blocked, but on a global scale this 'now' is hardly applicable.
However, things are changing very quickly and give guarantees that TSPU will not learn, somehow no one can detect these garbage bags, the benefit of such clients is becoming more and more and they use not only the WireGuard protocol, and randomizing these packages practically reduces to "no" classification capability. The theory is over.
