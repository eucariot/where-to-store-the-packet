9. Заключение
=============

Заключение
----------

| Что ещё сказать после 50 мегбайтов? Только то, что многое из того, что вы прочитали в этот раз - частные случаи, которые могут быть (и будут) несправедливы в других ситуациях.
| Как только сетевой инженер смещает свой фокус со стандартизированных протоколов в область обработки пакетов, он падает в пропасть бесконечных компромиссов, где нет универсальных ответов, нет RFC, нет исчерпывающих мануалов. И чем `глубже <https://pikabu.ru/story/naskolko_gluboka_yeta_peshchera_7041398>`_ он падает, тем страшнее становится разнообразие деталей и нюансов.

| Эта книга планировалась небольшой заметкой о буферах - хотелось копнуть неглубокую ямку и выяснить, чем отличаются Shallow Buffer от Deep. Всё началось с небольшой `странички <https://people.ucsc.edu/~warner/buffer.html>`_, подбивающей информацию о размерах буферов. А потом ссылочка за ссылочкой и размотался клубок. Стало понятно, что без разбора типов чипов не обойтись, дальше пришлось углубиться в архитектуру. Здесь бы и тормознуть, но верёвка уже оборвалась. 

----

Полезные ссылки
---------------

В этот раз хоть под кат убирай. Но, поверьте, я оставил тут только самые хорошие источники, прочитанные лично моими глазами и отобранные лично моими руками.

    * **Архитектура сетевых устройств**

        * `Anatomy of Internet Routers <https://www.cisco.com/c/dam/global/hr_hr/assets/ciscoconnect/2013/pdfs/Anatomy_of_Core_Network_Elements_Josef_Ungerman.pdf>`_
        * `Cisco Nexus 3000 Switch Architecture <https://people.ucsc.edu/~warner/Bufs/BRKDCN-3734.pdf>`_
        * `Juniper Hardware Architecture <https://habr.com/ru/post/307696/>`_
        * `Hardware Defined Networking <https://www.amazon.com/Hardware-Defined-Networking-Brian-Petersen/dp/B075LY9CNM>`_
        * `Как сделать коммутатор? <https://linkmeup.ru/blog/401.html>`_
        * `Сети для самых маленьких. Часть четырнадцатая. Путь пакета <https://linkmeup.ru/blog/312.html>`_
    
    * **Архитектура ASIC**

        * `Packet Pushers. Understanding ASICs For Network Engineers (Pete Lumbis <https://www.youtube.com/watch?v=Ti3t9OAZL3g)>`_
        * `Cisco Enterprise ASICs <https://www.ciscolive.com/c/dam/r/ciscolive/us/docs/2016/pdf/BRKARC-3467.pdf>`_
        * `Broadcom Ships Jericho2 <https://people.ucsc.edu/~warner/Bufs/CSG-DNX-Switching-J2%20Feb%2016%202018.pdf>`_
        * `Broadcom Launches Another Tomahawk Into The Datacenter <https://www.nextplatform.com/2019/12/12/broadcom-launches-another-tomahawk-into-the-datacenter/>`_
        * `Programmable Pipeline <https://platformlab.stanford.edu/Seminar%20Talks/programming_line_rate_switches.pdf>`_
        * `The Most Important Development Of This Century <https://seekingalpha.com/article/4276568-important-development-of-this-century>`_
        * `Understanding chiplet in one article <https://www.mccoycomponents.com/blog/view/understanding-chiplet-in-one-article>`_
        * `Advanced_packaging_five_trends_to_watch_in_2017.aspx# Advanced packaging: five trends to watch in 2017 <https://beta.electronicproducts.com/Packaging_and_Hardware/Device_Packaging/>`_
        * `Fan Out – Simple to Complex <http://semicontaiwan.org/zh/sites/semicontaiwan.org/files/data16/docs/6.%20ASE_John%20Hunt.pdf>`_

    * **Программируемость**

        * `Design Principles for Packet Parsers <http://klamath.stanford.edu/~nickm/papers/ancs48-gibb.pdf>`_.
        * `Fast Programmable Match-Action Processing in Hardware for SDN <https://www2.cs.duke.edu/courses/fall19/compsci514/papers/rmt-sigcomm2013.pdf>`_
        * `P4 Tutorial, Hot Chips 2017 <https://www.hotchips.org/wp-content/uploads/hc_archives/hc29/HC29.20-Tutorials-Pub/HC29.20.1-P4-Soft-Net-Pub/HC29.21.100-P4-Tutorial.pdf>`_

    * **Архитектура памяти**

        * `Packet Buffers <https://people.ucsc.edu/~warner/buffer.html>`_. Отсюда по ссылкам разворачиваются разнообразные материалы очень глубоко
        * `An Update on Router Buffering <https://people.ucsc.edu/~warner/Bufs/Buffering-WP_August_2017.pdf>`_
        * `NCS 5500 Buffering Architecture <https://xrdocs.io/ncs5500/blogs/2018-05-07-ncs-5500-buffering-architecture/>`_
        * `Cisco Nexus 5000 Series Switches <https://www.cisco.com/c/en/us/products/collateral/switches/nexus-5020-switch/white_paper_c11-465436.html>`_. Cut-through and Store-and-Forward
        * `Understanding CoS Flow Control (Ethernet PAUSE and PFC <https://www.juniper.net/documentation/en_US/junos/topics/concept/cos-qfx-series-congestion-notification-understanding.html#jd0e554)>`_
        * `Quality of Service.Headroom buffers <https://github.com/Mellanox/mlxsw/wiki/Quality-of-Service>`_.  

    * **Реализации очередей**

        * `Strategies of packet buffering inside Routers <https://archive.nanog.org/sites/default/files/wednesday_tutorial_szarecki_packet-buffering.pdf>`_
        * `Understanding CoS Virtual Output Queues (VOQs) on QFX10000 Switches <https://www.juniper.net/documentation/en_US/junos/topics/concept/cos-qfx-series-voq-understanding.html>`_
        * `What is VOQ and why you should care? <https://forums.juniper.net/t5/forums/recentpostspage/post-type/message/category-id/Blogs/user-id/101479>`_

    * **Deep Buffers**

        * `Not all deep buffer switches are created equal <https://forums.juniper.net/t5/Enterprise-Cloud-and/Not-all-deep-buffer-switches-are-created-equal/ba-p/318393>`_
        * `Arista’s Big Buffer B.S. <https://packetpushers.net/aristas-big-buffer-b-s/>`_
        * `Speeding Applications in Data Center Networks. The Interaction of Buffer Size and TCP Protocol Handling and its Impact on Data-Mining and Large Enterprise IT Traffic Flows <http://miercom.com/pdf/reports/20160210.pdf>`_

    * `Data Center TCP (DCTCP): TCP Congestion Control for Data Centers <https://tools.ietf.org/html/rfc8257>`_    
    * `Understanding Microburst <https://support.huawei.com/enterprise/en/doc/EDOC1100086962>`_
    * Ну и немного мотивационных видео от Broadcom

        * `Introduction to Broadcom's Switch Portfolio <https://www.youtube.com/watch?v=t_fwyKs1wJ0&>`_
        * `Broadcom Trident4: Disrupting the Enterprise Data Center & Campus <https://www.youtube.com/watch?v=2HvxxK39BXM>`_
        * `Broadcom Tomahawk4: Industry's Highest Bandwidth Chip <https://www.youtube.com/watch?v=B-COGMbaUg4>`_
        * `Jericho2: Driving Merchant Silicon Revolution <https://www.youtube.com/watch?v=JUgyaSoErlQ>`_

----

Спасибы
-------

    * Андрею Глазкову (glazgoo) за рецензию и дельные замечания о Shared Buffers и коммерческих чипах
    * Михаилу Соколову (insektazz) за разъяснения об устройстве чипов, SerDes и Silicon Photonics
    * Александру Клименко (v0lk) за обнаружение точек роста в вопросах Admission Control, Alpha, Pipeline'ов и минусов DCTCP
    * Александру Азимову (mitradir) за комментарии о Lossless Ethernet
    * Дмитрию Афанасьеву (fl0w) за дополнения ко всем частям статьи
    * Виталию Венгловскому (AllTheThingsUndone) за наставление на путь в вопросах On-Chip Buffer, Packaging и других
    * Наташе Самойленко за помощь с RTD. Благодаря ей вы можете скачать эту книгу в PDF.
    * Артёму Чернобаю за КДПВ

    Особо благодарных просим задержаться и пройти на `Патреон <https://www.patreon.com/linkmeup?ty=h>`_.

        .. image:: https://fs.linkmeup.ru/images/patreon.jpg           
           :align: center
           :target: https://www.patreon.com/linkmeup?ty=h