# Pwnagotchi

<p align="center">
    <a href="https://github.com/evilsocket/pwnagotchi/releases/latest"><img alt="Release" src="https://img.shields.io/github/release/evilsocket/pwnagotchi.svg?style=flat-square"></a>
    <a href="https://github.com/evilsocket/pwnagotchi/blob/master/LICENSE.md"><img alt="Software License" src="https://img.shields.io/badge/license-GPL3-brightgreen.svg?style=flat-square"></a>
    <a href="https://github.com/evilsocket/pwnagotchi/graphs/contributors"><img alt="Contributors" src="https://img.shields.io/github/contributors/evilsocket/pwnagotchi"/></a>
    <a href="https://travis-ci.org/evilsocket/pwnagotchi"><img alt="Travis" src="https://img.shields.io/travis/evilsocket/pwnagotchi/master.svg?style=flat-square"></a>
    <a href="https://invite.pwnagotchi.ai/"><img alt="Slack" src="https://invite.pwnagotchi.ai/badge.svg"></a>
    <a href="https://community.pwnagotchi.ai/"><img alt="Forum" src="https://img.shields.io/discourse/posts?server=https%3A%2F%2Fcommunity.pwnagotchi.ai%2F&style=flat-square"></a>
    <a href="https://twitter.com/intent/follow?screen_name=pwnagotchi"><img src="https://img.shields.io/twitter/follow/pwnagotchi?style=social&logo=twitter" alt="follow on Twitter"></a>
</p>

[Pwnagotchi](https://pwnagotchi.ai/) bir [A2C](https://hackernoon.com/intuitive-rl-intro-to-advantage-actor-critic-a2c-4ff545978752)-tabanlı "AI" kaldıraç [bettercap](https://www.bettercap.org/) yakaladığı kırılabilir WPA anahtar malzemesini en üst düzeye çıkarmak için çevresindeki WiFi ortamından öğrenen (pasif olarak veya kimlik doğrulama ve ilişkilendirme saldırıları gerçekleştirerek). Bu materyal, tarafından desteklenen herhangi bir el sıkışma biçimini içeren PCAP dosyaları olarak toplanmıştır. [hashcat](https://hashcat.net/hashcat/), içermek [PMKIDs](https://www.evilsocket.net/2019/02/13/Pwning-WiFi-networks-with-bettercap-and-the-PMKID-client-less-attack/), 
tam ve yarım WPA tokalaşmaları.

![ui](https://i.imgur.com/X68GXrn.png)

Sadece oynamak yerine [Super Mario yada Atari oyunları](https://becominghuman.ai/getting-mario-back-into-the-gym-setting-up-super-mario-bros-in-openais-gym-8e39a96c1e41?gi=c4b66c3d5ced) çoğu takviye gibi öğrenmeye dayalı "AI" *(yawn)*, Pwnagotchi melodileri [parametreleri](https://github.com/evilsocket/pwnagotchi/blob/master/pwnagotchi/defaults.toml) maruz kaldığınız ortamlarda **WiFi özelliklerini daha iyi hale getirmek** için zamanla.

Daha spesifik olarak, Pwnagotchi bir [MLP özellik çıkarıcılı LSTM](https://stable-baselines.readthedocs.io/en/master/modules/policies.html#stable_baselines.common.policies.MlpLstmPolicy) için politika ağı olarak [A2C temsilcisi](https://stable-baselines.readthedocs.io/en/master/modules/a2c.html). A2C'ye aşina değilseniz, işte burada [çok iyi bir giriş açıklaması](https://hackernoon.com/intuitive-rl-intro-to-advantage-actor-critic-a2c-4ff545978752) (komik biçimde!) Pwnagotchi'nin nasıl öğrendiğinin arkasındaki temel ilkeler. (Pwnagotchi'nin nasıl öğrendiği hakkında daha fazla bilgiyi [Usage](https://www.pwnagotchi.ai/usage/#training-the-ai) doc.)

**Unutmayın:** Alışılmış RL simülasyonlarının aksine, Pwnagotchi zamanla öğrenir. Bir Pwnagotchi için zaman, çağlarla ölçülür; tek bir çağ, kaç erişim noktasının ve istemci istasyonunun görünür olduğuna bağlı olarak birkaç saniyeden dakikalara kadar sürebilir. Pwnagotchi'nizin başlangıçta inanılmaz derecede iyi performans göstermesini beklemeyin, çünkü öyle olacaktır. [keşfetmek](https://hackernoon.com/intuitive-rl-intro-to-advantage-actor-critic-a2c-4ff545978752) birkaç kombinasyon [anahtar parametreler](https://www.pwnagotchi.ai/usage/#training-the-ai) başlangıç ​​dönemlerinde maruz kaldığınız belirli bir ortamı ayarlamak için ideal ayarlamaları belirlemek için ... ancak ** size sıkıcı olduğunu söylediğinde Pwnagotchi'nizi dinleyin!** Yanınızda yeni WiFi ortamlarına getirin ve yeni gözlemlemesini sağlayın ağlar ve yeni el sıkışmaları yakalayın; göreceksiniz. :)

Yakın fiziksel yakınlıktaki birden çok birim, mevcut dot11 standardının üzerine inşa ettiğim bir parazit protokolünü kullanarak özel bilgi öğeleri yayınlayarak birbirleriyle "konuşabilir" ve varlıklarını birbirlerine duyururlar. Zamanla, birlikte eğitilmiş iki veya daha fazla birim, birbirlerinin varlığını tespit ettikten sonra, optimum pwnage için mevcut kanalları aralarında bölerek işbirliği yapmayı öğreneceklerdir.

## Belgeler

https://www.pwnagotchi.ai

## Linkler

&nbsp; | Resmi Bağlantılar
---------|-------
Website | [pwnagotchi.ai](https://pwnagotchi.ai/)
Forum | [community.pwnagotchi.ai](https://community.pwnagotchi.ai/)
Slack | [pwnagotchi.slack.com](https://invite.pwnagotchi.ai/)
Subreddit | [r/pwnagotchi](https://www.reddit.com/r/pwnagotchi/)
Twitter | [@pwnagotchi](https://twitter.com/pwnagotchi)

## Lisans

`pwnagotchi` ile yapılır ♥ [@evilsocket](https://twitter.com/evilsocket) ve [amazing dev team](https://github.com/evilsocket/pwnagotchi/graphs/contributors). GPL3 lisansı altında yayınlanmıştır.
