<div align="center">

<a href="https://usemagpie.ai"><img src="site/public/img/icon-256.png" width="112" alt="magpie"></a>

# magpie

### Her ajanın modeli. Tek bir yerde.

**Kimi üzerinde Claude Code. DeepSeek üzerinde Codex. GLM üzerinde Gemini CLI. ChatGPT aboneliğinle OpenCode.**<br>
Hepsini menü çubuğundan değiştir. Tek bir yerel ağ geçidi (gateway) hepsine hizmet eder,<br>
bir kota bittiğinde de sessizce bir sonraki hesabına geçer.

[![Release](https://img.shields.io/github/v/release/yetone/magpie-releases?label=release&color=111111)](https://github.com/yetone/magpie-releases/releases/latest) [![Stars](https://img.shields.io/github/stars/yetone/magpie?style=flat&color=111111)](https://github.com/yetone/magpie/stargazers) [![Discord](https://img.shields.io/badge/Discord-join-5865F2?logo=discord&logoColor=white)](https://discord.gg/vGSnD3ZKQF) [![License](https://img.shields.io/badge/license-MIT-111111)](LICENSE)<br>
![macOS](https://img.shields.io/badge/macOS-000000?logo=apple&logoColor=white) ![Windows](https://img.shields.io/badge/Windows-0078D4?logo=windows&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![Termux](https://img.shields.io/badge/Termux-000000?logo=android&logoColor=white)

magpie'ye ve açık kaynak topluluğuna verdiği destek için [Kimi](https://usemagpie.ai/go/kimi/readme)'ye teşekkürler.

<sub>Sponsorlar</sub>

<a href="https://usemagpie.ai/go/zerotoken/readme"><picture><source media="(prefers-color-scheme: dark)" srcset="site/public/img/sponsor-zerotoken-dark.svg"><img src="site/public/img/sponsor-zerotoken.svg" width="200" height="50" alt="零词元"></picture></a>&emsp;&emsp;<a href="https://usemagpie.ai/go/apikeyfan/readme"><picture><source media="(prefers-color-scheme: dark)" srcset="site/public/img/sponsor-apikeyfan-dark.svg"><img src="site/public/img/sponsor-apikeyfan.svg" width="200" height="50" alt="APIKEY.FAN"></picture></a><br>
<a href="https://usemagpie.ai/go/wandapi/readme"><picture><source media="(prefers-color-scheme: dark)" srcset="site/public/img/sponsor-wandapi-dark.svg"><img src="site/public/img/sponsor-wandapi.svg" width="200" height="50" alt="WandAPI"></picture></a>&emsp;&emsp;<a href="https://usemagpie.ai/go/aigocode/readme"><picture><source media="(prefers-color-scheme: dark)" srcset="site/public/img/sponsor-aigocode-readme-dark.png"><img src="site/public/img/sponsor-aigocode-readme.png" width="200" height="50" alt="AIGoCode"></picture></a><br>
<a href="https://usemagpie.ai/go/modelgo/readme"><picture><source media="(prefers-color-scheme: dark)" srcset="site/public/img/sponsor-modelgo-dark.svg"><img src="site/public/img/sponsor-modelgo.svg" width="200" height="50" alt="ModelGo"></picture></a>

**[İndir](https://usemagpie.ai)** &nbsp;·&nbsp; **[Belgeler](https://usemagpie.ai/docs/start)** &nbsp;·&nbsp; **[Başvuru](docs/reference.md)** &nbsp;·&nbsp; **[Eklentiler](https://github.com/magpie-community/plugins)** &nbsp;·&nbsp; **[Discord](https://discord.gg/vGSnD3ZKQF)** &nbsp;·&nbsp; [English](README.md) · [简体中文](README.zh-CN.md) · **Türkçe**

<br>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/agents-dark.png">
  <img src="site/public/img/agents-light.png" width="900" alt="magpie'nin Ajanlar sayfası: Kimi K3 üzerinde Claude Code, DeepSeek V4 Pro üzerinde Codex, GLM-5.3 üzerinde Gemini CLI; hepsi tek bir listeden seçiliyor">
</picture>

</div>

<br>

> 🇹🇷 Bu, [yetone/magpie](https://github.com/yetone/magpie) README'sinin topluluk tarafından yapılmış Türkçe çevirisidir. Güncel ve resmi bilgi için [İngilizce sürüme](README.md) bak.

## magpie sana göre mi?

Her ajan modelini kendi dosyasında, kendi formatında, kendi anahtarları ve temel URL'leriyle tutar. Parasını ödediğin bir abonelik tek bir ajanda çalışır, başka hiçbir yerde çalışmaz. magpie bunların hepsini tek bir uygulamanın ve tek bir yerel ağ geçidinin arkasına toplar:

- **Herhangi bir ajan için herhangi bir modeli** tek bir listeden seç. magpie, ajanın kendi yapılandırmasında yalnızca önemli olan tek anahtarı değiştirir.
- **Tek bir sağlayıcıyı her yerde kullan**: bir API anahtarı, yerel bir model ya da giriş yaptığın Claude, ChatGPT, Copilot, Gemini veya Grok aboneliği.
- **Kota bitince durma**: sağlayıcının bir sonraki hesabı devralır, bir yönlendirme grubu da başka bir modele ya da sağlayıcıya geçer; ajan hatayı hiç görmez. Tek hesabın varsa ve grup kurmadıysan geçilecek bir yer yoktur, hata ajana ulaşır.
- **Gizli bilgilerini sağlayıcının sunucularından uzak tut**: **Ayarlar → Gizlilik** bölümünden maskelemeyi açtığında (varsayılan olarak kapalı), istemdeki anahtarlar, şifreler ve e-postalar istek bilgisayarından çıkmadan önce maskelenir, yanıtta da geri yerine konur.

Birden fazla ajan, birden fazla sağlayıcı ya da birden fazla hesap kullanıyorsan tam sana göre. Tek bir ajanı kendi sağlayıcısının aboneliğiyle kullanıyorsan ve bu sana yetiyorsa, buna ihtiyacın yok.

macOS, Windows ve Linux'ta (menü çubuğu uygulaması, pencere, TUI, web arayüzü ve CLI), Docker'da ve Termux'ta çalışır.

## Hızlı başlangıç

**1 · Kur.** Uygulamayı **[usemagpie.ai](https://usemagpie.ai)** adresinden indir ya da şunu çalıştır:

```sh
curl -fsSL https://usemagpie.ai/install.sh | sh
```

<sub>Mac sürümleri imzalı ve Apple onaylıdır (notarized); her sürüm dosyası bir GitHub Actions derleme doğrulaması taşır (`gh attestation verify <file> -R yetone/magpie-releases`) ve her sürüm kendini günceller. Linux'ta betik masaüstü uygulamasını kurar; masaüstünde WebKitGTK 4.1 yoksa önce onu paket yöneticinle kurar (sudo şifreni sorar). Masaüstü yoksa ya da soru sorulabilecek bir terminal yoksa terminal sürümünü kurar ve hangi paketi eklemen gerektiğini söyler. `--gui` veya `--tui` ile seçim yapabilirsin. Güvenlik duvarı arkasındaysan `--proxy` ya da `--mirror` kullan. Alternatif olarak `go install github.com/yetone/magpie@latest` ya da [Docker imajı](https://usemagpie.ai/docs/docker). magpie'yi kaldırmak için `curl -fsSL https://usemagpie.ai/install.sh | sh -s -- --uninstall`: önce ajanlarını eski haline getirir, sonra betiğin kurduklarını kaldırır (magpie zaten silinmişse, ajanları geri almak için bir tane indirir). `~/.config/magpie` içindeki ayarların, `--purge` eklemedikçe silinmez.</sub>

**2 · Bir sağlayıcı ekle.** magpie'yi aç ve **Providers → Add provider** bölümüne git. Bir hazır ayar seçip anahtarını yapıştır ya da bir abonelikle giriş yap.

**3 · Bir model seç**: **Agents** sayfasında her ajan için. Yeni bir oturum başlattığında ajan yeni modeli kullanır.

Ya da hepsini terminalden yap:

```sh
magpie provider add deepseek sk-…              # hazır ayar için sadece anahtar yeter
magpie claude deepseek/deepseek-v4-pro          # DeepSeek üzerinde Claude Code
magpie codex moonshot/kimi-k2.5                 # Kimi üzerinde Codex
magpie group add "Opus anywhere" models=claude/claude-opus-5-5,copilot/claude-opus-5.5 routing=smart
magpie claude group/opus-anywhere               # abonelikler arasında yedeğe geçer
magpie save work && magpie use work             # profiller
magpie quota                                    # her planda kalan kota
magpie settings set theme dark                  # her Ayarlar seçeneği, terminalden
magpie tool generate_image "a magpie, watercolour" -o hero.png   # magpie'nin görsel, görme ve arama araçları, doğrudan
magpie tui                                      # her şey, terminalde
```

magpie, ajanlarının giriş yaptığı abonelikleri onların giriş bilgilerini okuyarak bulur (Claude Code'un ve Codex'in dosyaları, Anahtar Zinciri). Bunları okumasını istemiyorsan Ayarlar → Gizlilik → *Subscription accounts* seçeneğini kapat ya da `magpie accounts discovery off` çalıştır (`on` geri açar). `MAGPIE_NO_ACCOUNTS=1`, kayıtlı ayarı değiştirmeden tek bir çalıştırma için kapatır. API anahtarlı sağlayıcılar her iki durumda da çalışır.

## Desteklenen ajanlar

<table>
<tr><td>

Claude Code · Claude Desktop · Claude Science · Codex · Gemini CLI · Antigravity CLI · Dim · OpenCode · OpenChamber · MiMo Code · DevEco Code · Pi · oh-my-pi · StepCode · MothX · PenguinHarness · Aside · OmO · Prime Agent · mu · Goose · Cursor CLI · Cursor Private Inference · Zed · VS Code Chat · VS Code Insiders · VSCodium Chat · Zoo Code · JetBrains Air · Air (JetBrains IDEs) · Copilot (JetBrains) · Copilot CLI · Crush · DeepSeek Harness · Reasonix Studio · Command Code · fx · Devin · Hermes Agent · Mister Morph · Kimi Code · jcode · Mistral Vibe · Qwen Code · Muse Code · Empryo · nanobot · miniQ · Paimon · MiniMax Code · Droid · Cline · Qoder · Qoder CN · Grok Build · Grok App · ZCode · WorkBuddy · WorkBuddy AI · CodeBuddy · Pencil · Paseo · OpenPencil · OpenBot · Craft Agents · Tuanjie Cowork · NewMax · LiveAgent · Raycast · Kiro Crew · OpenMausBot · T3 Code · OpenHanako · AtomCode · Snow CLI · Alma · Shelley · Cindy · Lody · AionUi · Cherry Studio · Ante · AstrBot · QwenPaw · OpenClaw · Avibe · Kun

</td></tr>
</table>

magpie yalnızca bilgisayarında kurulu olan ajanları gösterir; bazılarının kurulum notları [başvuru belgesinde](docs/reference.md#notes-on-some-agents). Temel URL (base URL) kabul eden başka her şey de ağ geçidini kullanabilir:

```sh
export OPENAI_BASE_URL=http://127.0.0.1:3425/v1     OPENAI_API_KEY=magpie
export ANTHROPIC_BASE_URL=http://127.0.0.1:3425     ANTHROPIC_API_KEY=magpie
export GOOGLE_GEMINI_BASE_URL=http://127.0.0.1:3425 GEMINI_API_KEY=magpie
```

## Parçalar nasıl birleşiyor

`127.0.0.1:3425` adresindeki ağ geçidi OpenAI Chat, OpenAI Responses, Anthropic Messages ve Gemini protokollerini konuşur ve aralarında çeviri yapar; akış (streaming), araç çağrıları ve akıl yürütme (reasoning) dahil.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/architecture-dark.svg">
  <img src="site/public/img/architecture.svg" alt="magpie'nin yapısı: ajanların istekleri 127.0.0.1:3425 adresindeki magpie ağ geçidine gönderir; ağ geçidi bunları yönlendirme grupları ve eklentiler üzerinden API anahtarlarına, aboneliklere ve yerel modellere yönlendirir.">
</picture>


## Neler yapar

### Her model, her ajan

Bir değere tıkla, aranabilir bir liste açılır: eklediğin her sağlayıcının her modeli, `sağlayıcı/model` biçiminde. Ajanın yapılandırması atomik olarak yeniden yazılır; yorumları, sırası ve biçimlendirmesi olduğu gibi kalır. **Profiller** her ajanın kurulumunu tek bir ad altında kaydeder ("Bütçe", "Odak") ve hepsini tek hamlede geri getirir. Her ajanın kendi kısa model listesi de olabilir; profil bu listeyi de saklar.

<table>
<tr>
<td width="50%">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/panel-dark.png">
  <img src="site/public/img/panel-light.png" alt="Menü çubuğu paneli">
</picture>
</td>
<td width="50%">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/picker-dark.png">
  <img src="site/public/img/picker-light.png" alt="Model seçici">
</picture>
</td>
</tr>
</table>

### Gizlilik maskelemesi

Ajanlar okudukları şeyleri isteme (prompt) koyar: bir `.env`, bir yapılandırma dosyası, içinde token olan bir log. Maskeleme açıkken magpie, istek bilgisayarından çıkmadan önce bu değerleri yer tutucularla değiştirir ve yanıtta geri koyar. Ajanın ve dosyaların gerçek değerleri tutmaya devam eder; sağlayıcı onları hiç görmez.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/masking-dark.png">
  <img src="site/public/img/masking-light.png" width="900" alt="Insights › Masking: 7 günde sağlayıcılardan saklanan 5.812 değer; Claude Code ve Codex'ten magpie üzerinden OpenAI, Kimi ve DeepSeek'e akış ve her isteğin maskelenmiş değerleri">
</picture>

| | |
| :-- | :-- |
| **İki yolla bulunur** | Kesin olanlar için kurallar (API anahtarları, özel anahtarlar, token'lar, e-postalar ve sağlama toplamı tutan kart ve kimlik numaraları); istersen, hiçbir kuralın bulamayacağı isimler, adresler ve şifreler için bu bilgisayarda çalışan bir model (1,6 GB indirme, CPU üzerinde) |
| **Her yerde geri konur** | Bir değer `{{API_KEY_k3v9x2mq}}` gibi bir yer tutucuya dönüşür ve yanıttaki her yer tutucu tekrar değerine döner: akış halindeki metin ve araç çağrısı argümanları da dahil, yani ajanın çalıştırdığı komutta gerçek anahtar olur |
| **Hiçbir şey bozulmaz** | Bir değer her seferinde aynı yer tutucuyu alır; böylece konuşma, istem önbelleği ve düşünme imzaları geçerli kalır. Bir kez maskelenen değer, sonra nerede görünürse görünsün maskelenir |
| **Asla diske yazılmaz** | Değerler yalnızca bellekte tutulur. Kayıt, her değerin türünü, uzunluğunu ve ilk karakterlerini saklar. Maskeleme açıksa ve çalışamazsa istek bekletilir (503), asla olduğu gibi gönderilmez |
| **Kontrol edebilirsin** | **Insights › Masking**, değiştirdiği her isteği ve sağlayıcının yerine ne aldığını yan yana listeler; Ayarlar'daki **Try it** bir metnin neye dönüşeceğini gösterir |
| **Senin kuralların** | Gizli bilgiler ve kişisel veriler ayrı ayrı açılıp kapatılabilir; daha ince türler (pasaport, IBAN, MAC, genel IP…), kendi kelimelerin ve kalıpların; bulunan bir değerin maskelenmesi, sadece uyarı verilmesi ya da isteğin durdurulması (**Mask**, **Warn**, **Block**) |

Bedeli: model anahtarı değil `{{API_KEY_…}}` ifadesini görür; dolayısıyla değerin kendisiyle ilgili bir görev (bu token neden reddediliyor?) onunla yapılamaz. Böyle değerleri **Never mask** altına koy. Kurallar ara sıra yanılabilir; bunu Masking sayfasında görürsün. **Ayarlar → Gizlilik** bölümünden açana kadar kapalıdır. Örnekler için ayrılmış adlardaki e-postalar (`example.com`, `.test`, `.invalid`) olduğu gibi bırakılır.

### Sağlayıcılar

Bir hazır ayar seç, anahtarı yapıştır. Model listeleri sağlayıcıdan gelir; adlar ve akıl yürütme seviyeleri [models.dev](https://models.dev) üzerinden doldurulur. Yani bu sabah çıkan bir model, bir sonraki yenilemede seçicinde olur.

> **Hazır ayarlar arasında** Anthropic · OpenAI · Google Gemini · Google Vertex AI · Amazon Bedrock (runtime ve Mantle) · DeepSeek · Kimi · Zhipu GLM · MiniMax · StepFun · LongCat · Qwen · Baidu Qianfan · Tencent Cloud · Huawei Cloud MaaS · Volcengine Ark · Mistral · Voyage AI · Groq · Nous Portal · xAI · OpenRouter · Vercel AI Gateway · GMI Cloud · Together · Fireworks · Fireworks Nexus · SiliconFlow · NVIDIA NIM · ModelScope · Ollama · LM Studio … ve OpenAI ya da Anthropic uyumlu herhangi bir URL var.

**İçe aktarma (Import)**, CC Switch, Claude Code, Codex ve Alma'daki sağlayıcıları getirir. **[Add to magpie](https://usemagpie.ai/docs/import)** bağlantıları, bir sağlayıcının web sitesinin yapılandırmasını tek tıkla magpie'ye aktarmasını sağlar. Her anahtar ve her hesap kendi proxy'si üzerinden gidebilir.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/add-dark.png">
  <img src="site/public/img/add-light.png" width="900" alt="Sağlayıcı ekle: giriş yapılacak abonelikler, sağlayıcılar, aracılar ve yerel sunucular">
</picture>

### Abonelikler

Giriş yaptığın bir ajan, arkasında modeller olan bir aboneliktir; bu yüzden magpie onu diğer tüm ajanlara bir sağlayıcı olarak sunar. Abonelik başına birkaç hesap ekle, magpie aralarında yedeğe geçsin.

- **Claude**: gerçek yerel `claude` programını çalıştırır ve ajanının araçlarını MCP üzerinden köprüler
- **Codex / ChatGPT**: ChatGPT planındaki modeller, diğer tüm ajanlarda
- **GitHub Copilot**, **Gemini (Code Assist)**, **Antigravity** (kendi agy CLI'n üzerinden), **Grok (SuperGrok)** ve daha fazlası
- npm'deki **her OpenCode kimlik doğrulama eklentisi veya pi paketi**

**Günlük ısınma (Daily warm-up)**, her Claude ve ChatGPT hesabının 5 saatlik penceresini seçtiğin saatlerde ya da sonuncusu sıfırlandığı anda başlatır.

### Yönlendirme grupları

**Yönlendirme grubu**, bir ajanın tek bir model gibi seçtiği birkaç modeldir; örneğin `group/daily-coding`. Ağ geçidi istekleri tüm üyelerin anahtarlarına ve hesaplarına dağıtır:

| Mod | Ne yapar |
| :-- | :-- |
| **`smart`** | Kotası kalan abonelikler arasından en erken yenilenecek olanı kullanır; böylece sıfırlamada daha az kota boşa gider |
| **`order`** | İlk modeli yanıt veremeyene kadar kullanır, sonra bir sonrakine geçer |
| **`rotate`** | Her turda bir sonraki üyeye geçer |
| **`usage`** | Önce en az kullanılan üyeyi kullanır |
| **`pace`** | Sıfırlanana kadar saat başına haftasından en çok kalan hesabı kullanır |

Bir konuşma, sağlayıcının istem önbelleği değerli olduğu sürece **ona yanıt veren hesapta kalır**. Gruplar başka grupları içerebilir. **[Niyet yönlendirmesi (Intent routing)](https://usemagpie.ai/docs/intent)** ile seçtiğin küçük bir model her yeni turu okur; testler güçlü modele, hızlı sorular ucuz modele gider. Routing görünümü her kararı canlı gösterir.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/routing-dark.png">
  <img width="760" src="site/public/img/routing-light.png" alt="Routing görünümü: dört ajan magpie üzerinden yedi sağlayıcıya, canlı">
</picture>

<table>
<tr>
<td width="50%">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/intent-trace-dark.png">
  <img src="site/public/img/intent-trace-light.png" alt="Niyete göre yönlendirilen bir tur, adım adım açıklanmış">
</picture>
</td>
<td width="50%">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/nested-routing-dark.png">
  <img src="site/public/img/nested-routing-light.png" alt="Bir yönlendirme grubunun içinde başka bir yönlendirme grubu">
</picture>
</td>
</tr>
</table>

### Eklentiler

```sh
magpie plugin add opencode-gemini-auth   # npm'den bir OpenCode eklentisi
magpie plugin login google-plugin        # eklentinin kendi giriş akışı, magpie içinde
```

Eklentiler [Bun](https://bun.sh) üzerinde çalışır; Bun, bir eklenti ilk kez ihtiyaç duyduğunda indirilir. Bir eklenti giriş yapar, modellerini listeler ve her isteği yapar; ajanlar bu modelleri diğer sağlayıcıların modelleri gibi kullanır. **[magpie-community/plugins](https://github.com/magpie-community/plugins)** adresine göz at ya da [kendininkini yaz](https://usemagpie.ai/docs/plugins).

Bir eklenti aynı zamanda **ağ geçidi ara katmanı (middleware)** olabilir: her ajanın gönderdiğini ve geri aldığını gören JavaScript. `onRequest` bir isteği yeniden yazabilir ya da reddedebilir, `onEvent` akıştaki her olayı, `onResponse` ise yanıtın tamamını görür. Hata fırlatan ya da çok uzun süren bir kanca (hook) isteği olduğu gibi bırakır.

```js
// alias.middleware.js — magpie plugin add ./alias.middleware.js
export function onRequest(body, ctx) {
  if (body.model === "fast") return { ...body, model: "deepseek/deepseek-chat" };
}
```

<details>
<summary><b>Hazır ara katmanlar</b>; çoğu <a href="https://github.com/QuantumNous/new-api">New API</a>'nin kanalları için yaptığı şeyler, aynı JSON ile</summary>

<br>

| Paket | Ne yapar |
| :-- | :-- |
| `param-override` | New API'nin `param_override` özelliği: istek alanlarını koşullara göre ayarla, sil, taşı veya yeniden yaz ya da isteği reddet |
| `model-map` | New API'nin `model_mapping` özelliği: bir modeli başka bir adla gönder; yanıtlar istenen adı korur |
| `system-prompt` | Her isteğe ya da bazı ajanların veya modellerin isteklerine kendi sistem istemin |
| `word-guard` | New API'nin hassas kelime filtresi: kullanıcıların gönderdiklerinde ve yanıtlarda kelimeleri reddet veya maskele |
| `think-tags` | Yanıtlardan `<think>…</think>` kısmını çıkar ya da `reasoning_content` içeriğini yanıta ekle |

```sh
magpie plugin add @magpie-community/middleware-model-map
magpie plugin options model-map '{"mapping": {"fast": "deepseek/deepseek-chat"}}'
```

Bunları Plugins › Discover › Gateway middleware altında bulabilirsin. Bkz. [Gateway middleware](https://usemagpie.ai/docs/plugins#middleware).

</details>

### Kullanım ve maliyet

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="site/public/img/usage-dark.png">
  <img src="site/public/img/usage-light.png" width="900" alt="Kullanım sayfası: bakiyeler, token'lar, önbellek isabet oranı ve maliyet">
</picture>

| | |
| :-- | :-- |
| **Token'lar ve maliyet** | Token'lar, önbellek okuma ve yazmaları, akıl yürütme ve çağrılar; maliyet liste fiyatıyla dolar ya da yuan cinsinden; her model için kendi fiyatını belirleyebilirsin |
| **Kota** | Her anahtar, plan ve hesap için bakiyeler ve kota pencereleri (`magpie quota`) ve büyük kısmı kullanılmamış bir pencere yenilenmeden önce hatırlatma |
| **Oturumlar** | Her ajan konuşması maliyeti ve başlığıyla; tek tıkla terminalinde yeniden açılır |
| **Bağlam** | Her isteğin bağlam penceresinin ne kadar dolu olduğu, ne kadarının önbellekten geldiği ve onu neyin doldurduğu |
| **Faturalar** | Hesaba ve üst kaynak anahtarına göre; kendi gözlemlenebilirlik altyapına OTLP dışa aktarımı |

### Paylaşım

| | |
| :-- | :-- |
| **Yerel ağ** | *Share on local network* seçeneğini aç ve her istemciye kendi günlük, haftalık veya aylık token ve maliyet limiti olan adlandırılmış bir ağ geçidi anahtarı ver |
| **[Uzak magpie](https://usemagpie.ai/docs/remote)** | Bir dizüstü bilgisayar, masaüstündeki magpie'nin sağlayıcılarını, hesaplarını ve gruplarını kullanır, yine de kendi ajanlarını bağlar |
| **[Docker](https://usemagpie.ai/docs/docker)** | `ghcr.io/yetone/magpie` imajını bir sunucuda veya NAS'ta çalıştır ve web arayüzünden yönet |
| **Senkronizasyon** | Bir dosyaya yedekle ya da makineleri WebDAV (Nutstore, Nextcloud…), S3 veya şifrelenmiş bir GitHub deposu yedeği üzerinden senkronize et |

### Ayrıca

- **Kütüphane (Library)**: talimatları, MCP sunucularını, becerileri (skills) ve alt ajanları bir kez yaz; magpie bunları her ajanın dosyalarına onun formatında yazar ve yalnızca kendi yazdıklarını kaldırır.
- **Her model için web araması**: arama yapamayan bir model magpie'nin aramasını kullanır: arama yapabilen bir sağlayıcı ya da arama API'leri (Tavily, Brave, Exa, Firecrawl, You.com, DeepSeek, Volcengine üzerinde Doubao Search, Tencent Cloud üzerinde Yuanbao Search, TinyFish, SearXNG). Bunlar sürükleyip bıraktığın sırayla sorgulanır ve her biri anahtarı kaybolmadan kapatılabilir. Bir API birkaç anahtar tutabilir: aramalar sırayla bunları kullanır (ya da `pick=order` ile belirli sırayla), son zamanlarda reddedilen anahtar en son denenir ve Tavily anahtarları limitlerinden ne kadar kullandıklarını hem Ayarlar'da hem `magpie search` komutunda gösterir. Her ajan aynı aramayı bir MCP sunucusu olarak bağlayabilir; bir `web_search` aracı ve bir sayfayı URL'siyle okuyan bir `web_fetch` aracı ile.
- **Görseller ve video**: MCP üzerinden her ajan için seçtiğin modelle bir görsel aracı; Grok aboneliği veya MiniMax API anahtarıyla (MiniMax H3) videolar.
- **Ajanlar güncel kalır**: Agents sayfası her CLI'ın sürümünü gösterir, onu kurulduğu yöntemle günceller ve sende olmayanlar için kurulum komutlarını verir.
- **WSL**: Windows'ta WSL dağıtımlarının içindeki ajanlar da bağlanır ve oturumları sayılır.
- **Uyanık tutma (Keep awake)**, açık ve koyu tema ve [Omarchy](https://omarchy.org) üzerinde kendi temanın görünümü.

## Belgeler

| | |
| :-- | :-- |
| **[Başlarken](https://usemagpie.ai/docs/start)** | Rehberli tur |
| **[Başvuru](docs/reference.md)** | Her ajan, sağlayıcı seçeneği, ağ geçidi uç noktası, CLI komutu ve dosya |
| **[Eklentiler](https://usemagpie.ai/docs/plugins)** | Eklentileri kullan ve kendininkini yaz |
| **[Niyet yönlendirmesi](https://usemagpie.ai/docs/intent)** | Her turu ne istediğine göre yönlendir |
| **[İçe aktarma bağlantıları](https://usemagpie.ai/docs/import)** | Sağlayıcı web siteleri için "Add to magpie" butonları |
| **[Uzak magpie](https://usemagpie.ai/docs/remote)** | Bir magpie'nin sağlayıcılarını ve gruplarını diğer bilgisayarlarından kullan |
| **[Docker](https://usemagpie.ai/docs/docker)** | magpie'yi bir sunucuda veya NAS'ta çalıştır |

## Gizlilik

İstemlerin, yanıtların, anahtarların ve hesapların yalnızca kullandığın sağlayıcılara gider; [gizlilik maskelemesi](#gizlilik-maskelemesi) açıkken içlerindeki gizli bilgiler oraya bile gitmez. Yayınlanmış bir magpie sürümü günde bir kez kullanımda olduğunu bildirir: rastgele bir kimlik, sürümü ve sistemi, hangi ajanlar, sağlayıcılar ve modellerle kullanıldığı (magpie'nin kendi kimlikleriyle; kendi eklediğin bir sağlayıcı sadece `custom` olarak görünür), Discover'da listelenen eklentilerden hangilerinin kurulu olduğu (her birini kaç kişinin kullandığını gösterebilmek için) ve ekleme ekranında ilk sırada listelenen her iş ortağı için günde kaç kez gösterildiği, açıldığı ve eklendiği (yalnızca sayılar). İsim, URL, hesap, anahtar, istem ya da kullanım bilgisi yok. Bunun bir kısmını ya da tamamını **Ayarlar → Gizlilik** bölümünden veya `DO_NOT_TRACK=1` ile kapatabilirsin. Bir iş ortağının web sitesi ve anahtar bağlantıları `usemagpie.ai/go/…` üzerinden geçer ve tıklamayı sayar; usemagpie.ai ayrıca iş ortağı listesinin çekilme sayısını sayar. Sunucu bunları ayarlardan bağımsız olarak görür ama hiçbir kimlik veya adres saklamaz. Bir eklentinin, içe aktarma bağlantısının ya da kütüphanenin adını verdiği simgeler `usemagpie.ai/api/icon` üzerinden çekilir; böylece o sunucular senin adresini değil Cloudflare'in adresini görür. Sunucu yalnızca resmi iletir, hiçbir şey saymaz ve saklamaz. [Gizlilik sayfası](https://usemagpie.ai/docs/privacy), magpie'nin kendiliğinden gönderdiği her şeyi bir örnekle ve tüm ayarlarla listeler; kurallar [başvuru belgesinde](docs/reference.md#counting-users).

## Topluluk

Sorun, fikrin ya da görünmeyen bir model mi var? **[Discord](https://discord.gg/vGSnD3ZKQF)**'da bize anlat. Geri bildirimler orada toplanıyor.

**Bu depo pull request kabul etmiyor.** Yalnızca bakımcılar açabilir. Bir düzeltme ya da özellik istiyorsan Discord'da anlat, biz yapalım.

magpie seni bir yapılandırma dosyası daha düzenlemekten kurtardıysa, **bir ⭐ başkalarının da onu bulmasına yardımcı olur.**

<a href="https://star-history.com/#yetone/magpie&Date">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=yetone/magpie&type=Date&theme=dark">
    <img src="https://api.star-history.com/svg?repos=yetone/magpie&type=Date" width="600" alt="Yıldız geçmişi">
  </picture>
</a>

## Lisans

[MIT](LICENSE)

magpie'nin [Apache Magpie](https://magpie.apache.org) ya da [Apache Software Foundation](https://apache.org) ile bir bağlantısı yoktur.
