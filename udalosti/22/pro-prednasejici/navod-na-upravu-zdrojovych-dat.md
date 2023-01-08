# Návod na úpravu zdrojových dat

Naše konference je open-source a zdrojové datové sady (přednášející, přednášky, partneři atp.) jsou publikované ve formě Git repozitáře [`utxo-foundation/utxo`](https://github.com/utxo-foundation/utxo).&#x20;

Kdokoliv s [GitHub](https://github.com/) účtem může navrhnout úpravu těchto dat, a to relativně jednoduše přes GitHub rozhraní a mechanismu [Pull Request (PR)](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests), viz návod níže.

### Krok 1. - volba datové sady

Pro otevření souboru datové sady využijte odkaz na soubor (viz. tabulka níže) nebo soubor nalezněte přímo v [repozitáři](https://github.com/utxo-foundation/utxo/tree/master/spec/22).

| Název                | Popis                                            | Soubor                                                                                           |
| -------------------- | ------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| **Přednášející**     | Seznam všech přednášejících a jejich detaily     | ``[`speakers.yaml`](https://github.com/utxo-foundation/utxo/blob/master/spec/22/speakers.yaml)`` |
| **Události**         | Seznam všech událostí a jejich detaily           | ``[`events.yaml`](https://github.com/utxo-foundation/utxo/blob/master/spec/22/events.yaml)``     |
| **Partneři**         | Seznam všech partnerů a jejich detaily           | ``[`partners.yaml`](https://github.com/utxo-foundation/utxo/blob/master/spec/22/partners.yaml)`` |
| **Programové sekce** | Seznam všech programových sekcí a jejich detaily | ``[`tracks.yaml`](https://github.com/utxo-foundation/utxo/blob/master/spec/22/tracks.yaml)``     |

### Krok 2. - úprava dat

{% hint style="info" %}
K dokončení tohoto kroku musíte mít účet na [GitHub](https://github.com/) a musíte být přihlášení.
{% endhint %}

Jakmile máte otevřený soubor s datovou sadou - klikněte na ikonku tužky vpravo nad obsahem souboru "_Edit this file"_ (viz. obrázek níže).

Poté se vám otevře editor a vy můžete upravit, to co potřebujete.

Datové soubory jsou v lidsky čitelném značkovacím formátu [YAML](https://yaml.org/) ([návod v češtině](https://zdrojak.cz/clanky/yaml-serializacni-format-pro-ukladani-dat/)). V rámci rozšířených údajů (např. `speakers.bio`, `speakers.desc` nebo `events.description`) může být text dále formátován jako [Markdown](https://www.markdownguide.org/).

![](<../../../.gitbook/assets/Screenshot 2022-04-21 at 20.04.39.png>)

### Krok 3. - odeslání změn (fork & commit)

Jakmile provedete úpravu textu souboru, je nutné vaše změny uložit. Na konci stránky naleznete formulář a tlačítko "_Propose changes_".

Vyplnit stačí jen první pole, kde popíšete v pár slovech vaši změnu a musí být zvoleno "_Create a new branch for this commit and start a pull request_".

Po kliknutí na tlačítko "_Propose changes"_ se se provede fork repozitáře, a změny se projeví na vašem forku (commit).

![](<../../../.gitbook/assets/Screenshot 2022-04-21 at 20.08.02.png>)

### Krok 4. - vytvoření Pull Request

Další krok je jen vytvoření [Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) žádosti - po jeho odeslání se změny pošlou organizátorům ke schválení.

Vyplňte nadpis, tedy stručné shrnutí vašich změn a klikněte na "Create pull request". Hotovo.

![](<../../../.gitbook/assets/Screenshot 2022-06-01 at 0.04.42.png>)
