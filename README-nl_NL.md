# Het Beknopte TypeScript Boek

Het Beknopte TypeScript Boek biedt een uitgebreid en beknopt overzicht van de mogelijkheden van TypeScript. Het biedt heldere uitleg over alle aspecten van de nieuwste versie van de taal, van het krachtige typesysteem tot geavanceerde functies. Of je nu een beginner bent of een ervaren ontwikkelaar, dit boek is een onschatbare bron om je begrip van en vaardigheid in TypeScript te vergroten.

Dit boek is volledig gratis en Open Source.

Ik geloof dat technisch onderwijs van hoge kwaliteit voor iedereen toegankelijk moet zijn, en daarom houd ik dit boek gratis en open.

Als het boek je heeft geholpen een bug op te lossen, een lastig concept te begrijpen of verder te komen in je carrière, overweeg dan om mijn werk te steunen door te betalen wat je wilt (suggestie: 15 USD) of door een kopje koffie te sponsoren. Jouw steun helpt me om de inhoud up-to-date te houden en uit te breiden met nieuwe voorbeelden en diepere uitleg.

[![Buy Me a Coffee](https://img.shields.io/badge/buy_me_a_coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/simonepoggiali)

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=QW82ZS956XLFY&no_recurring=0&currency_code=EUR)

## Vertalingen

Dit boek is vertaald in verschillende talen, waaronder:

[Chinees](https://github.com/gibbok/typescript-book/blob/main/README-zh_CN.md)

[Italiaans](https://github.com/gibbok/typescript-book/blob/main/README-it_IT.md)

## Downloads en website

Je kunt ook de Epub-versie downloaden:

[https://github.com/gibbok/typescript-book/tree/main/downloads](https://github.com/gibbok/typescript-book/tree/main/downloads)

Een online versie is beschikbaar op:

[https://gibbok.github.io/typescript-book](https://gibbok.github.io/typescript-book)

## Inhoudsopgave

<!-- markdownlint-disable MD004 -->
- [Het Beknopte TypeScript Boek](#het-beknopte-typescript-boek)
  - [Vertalingen](#vertalingen)
  - [Downloads en website](#downloads-en-website)
  - [Inhoudsopgave](#inhoudsopgave)
  - [Inleiding](#inleiding)
  - [Over de auteur](#over-de-auteur)
  - [Introductie tot TypeScript](#introductie-tot-typescript)
    - [Wat is TypeScript?](#wat-is-typescript)
    - [Waarom TypeScript?](#waarom-typescript)
    - [TypeScript en JavaScript](#typescript-en-javascript)
    - [TypeScript Codegeneratie](#typescript-codegeneratie)
    - [Modern JavaScript Nu (Downleveling)](#modern-javascript-nu-downleveling)
  - [Aan de slag met TypeScript](#aan-de-slag-met-typescript)
    - [Installatie](#installatie)
    - [Configuratie](#configuratie)
    - [TypeScript Configuratiebestand](#typescript-configuratiebestand)
      - [target](#target)
      - [lib](#lib)
      - [strict](#strict)
      - [module](#module)
      - [moduleResolution](#moduleresolution)
      - [esModuleInterop](#esmoduleinterop)
      - [jsx](#jsx)
      - [skipLibCheck](#skiplibcheck)
      - [files](#files)
      - [include](#include)
      - [exclude](#exclude)
    - [importHelpers](#importhelpers)
    - [Advies voor migratie naar TypeScript](#advies-voor-migratie-naar-typescript)
  - [Het typesysteem verkennen](#het-typesysteem-verkennen)
    - [De TypeScript Language Service](#de-typescript-language-service)
    - [Structurele Typering](#structurele-typering)
    - [Fundamentele vergelijkingsregels van TypeScript](#fundamentele-vergelijkingsregels-van-typescript)
    - [Types als Verzamelingen](#types-als-verzamelingen)
    - [Een type toewijzen: Typedeclaraties en Type-assertions](#een-type-toewijzen-typedeclaraties-en-type-assertions)
      - [Typedeclaratie](#typedeclaratie)
      - [Type-assertion](#type-assertion)
      - [Ambient Declarations](#ambient-declarations)
    - [Property Checking en Excess Property Checking](#property-checking-en-excess-property-checking)
    - [Zwakke Types (Weak Types)](#zwakke-types-weak-types)
    - [Strikte controle van Object Literals (Freshness)](#strikte-controle-van-object-literals-freshness)
    - [Type Inference](#type-inference)
    - [Geavanceerdere Inferences](#geavanceerdere-inferences)
    - [Type Widening](#type-widening)
    - [Const](#const)
      - [Const Modifier op Type Parameters](#const-modifier-op-type-parameters)
      - [Const-assertion](#const-assertion)
    - [Expliciete Type-annotatie](#expliciete-type-annotatie)
    - [Type-vernauwing (Type Narrowing)](#type-vernauwing-type-narrowing)
      - [Voorwaarden](#voorwaarden)
      - [Throwing of returning](#throwing-of-returning)
      - [Discriminated Union](#discriminated-union)
      - [User-Defined Type Guards](#user-defined-type-guards)
  - [Primitieve Types](#primitieve-types)
    - [string](#string)
    - [boolean](#boolean)
    - [number](#number)
    - [bigInt](#bigint)
    - [Symbol](#symbol)
    - [null en undefined](#null-en-undefined)
    - [Array](#array)
    - [any](#any)
  - [Type-annotaties](#type-annotaties)
  - [Optionele Eigenschappen](#optionele-eigenschappen)
  - [Readonly Eigenschappen](#readonly-eigenschappen)
  - [Index Signatures](#index-signatures)
  - [Types Uitbreiden](#types-uitbreiden)
  - [Literal Types](#literal-types)
  - [Literal Inference](#literal-inference)
  - [strictNullChecks](#strictnullchecks)
  - [Enums](#enums)
    - [Numerieke enums](#numerieke-enums)
    - [String enums](#string-enums)
    - [Constante enums](#constante-enums)
    - [Reverse mapping](#reverse-mapping)
    - [Ambient enums](#ambient-enums)
    - [Berekende en constante leden](#berekende-en-constante-leden)
  - [Narrowing](#narrowing)
    - [typeof type guards](#typeof-type-guards)
    - [Truthiness narrowing](#truthiness-narrowing)
    - [Equality narrowing](#equality-narrowing)
    - [In-operator narrowing](#in-operator-narrowing)
    - [instanceof narrowing](#instanceof-narrowing)
  - [Toewijzingen (Assignments)](#toewijzingen-assignments)
  - [Control Flow Analysis](#control-flow-analysis)
  - [Type Predicates](#type-predicates)
  - [Gediscrimineerde Unies (Discriminated Unions)](#gediscrimineerde-unies-discriminated-unions)
  - [Het never Type](#het-never-type)
  - [Exhaustiveness checking](#exhaustiveness-checking)
  - [Object Types](#object-types)
  - [Tuple Type (Anoniem)](#tuple-type-anoniem)
  - [Named Tuple Type (Gelabeld)](#named-tuple-type-gelabeld)
  - [Vaste lengte Tuple](#vaste-lengte-tuple)
  - [Union Type](#union-type)
  - [Intersection Types](#intersection-types)
  - [Type Indexing](#type-indexing)
  - [Type van Waarde](#type-van-waarde)
  - [Type van Functie Return](#type-van-functie-return)
  - [Type van Module](#type-van-module)
  - [Mapped Types](#mapped-types)
  - [Mapped Type Modifiers](#mapped-type-modifiers)
  - [Conditional Types](#conditional-types)
  - [Distributieve Conditional Types](#distributieve-conditional-types)
  - [infer Type-inference in Conditional Types](#infer-type-inference-in-conditional-types)
  - [Vooraf gedefinieerde Conditional Types](#vooraf-gedefinieerde-conditional-types)
  - [Template Union Types](#template-union-types)
  - [Any type](#any-type-1)
  - [Unknown type](#unknown-type-1)
  - [Void type](#void-type-1)
  - [Never type](#never-type-1)
  - [Interface en Type](#interface-en-type)
    - [Gemeenschappelijke Syntaxis](#gemeenschappelijke-syntaxis)
    - [Basis Types](#basis-types)
    - [Objecten en Interfaces](#objecten-en-interfaces)
    - [Union en Intersection Types](#union-en-intersection-types)
  - [Ingebouwde Type Primitieven](#ingebouwde-type-primitieven)
  - [Veelvoorkomende Ingebouwde JS Objecten](#veelvoorkomende-ingebouwde-js-objecten)
  - [Overloads](#overloads)
  - [Samenvoegen en Uitbreiden (Merging and Extension)](#samenvoegen-en-uitbreiden-merging-and-extension)
  - [Verschillen tussen Type en Interface](#verschillen-tussen-type-en-interface)
  - [Class](#class)
    - [Algemene Class Syntaxis](#algemene-class-syntaxis)
    - [Constructor](#constructor)
    - [Private en Protected Constructoren](#private-en-protected-constructoren)
    - [Access Modifiers](#access-modifiers)
    - [Get en Set](#get-en-set)
    - [Auto-Accessors in Classes](#auto-accessors-in-classes)
    - [this](#this)
    - [Parameter Eigenschappen](#parameter-eigenschappen)
    - [Abstracte Classes](#abstracte-classes)
    - [Met Generics](#met-generics)
    - [Decorators](#decorators)
      - [Class Decorators](#class-decorators)
      - [Property Decorators](#property-decorators)
      - [Method Decorators](#method-decorators)
      - [Getter en Setter Decorators](#getter-en-setter-decorators)
      - [Decorator Metadata](#decorator-metadata)
    - [Overerving (Inheritance)](#overerving-inheritance)
    - [Statics](#statics)
    - [Property initialisatie](#property-initialisatie)
    - [Method overloading](#method-overloading)
  - [Generics](#generics)
    - [Generic Type](#generic-type)
    - [Generic Classes](#generic-classes)
    - [Generic Constraints](#generic-constraints)
    - [Generic contextuele narrowing](#generic-contextuele-narrowing)
  - [Erased Structural Types](#erased-structural-types)
  - [Namespacing](#namespacing)
  - [Symbols](#symbols)
  - [Triple-Slash Directives](#triple-slash-directives)
  - [Type Manipulatie](#type-manipulatie)
    - [Types maken van Types](#types-maken-van-types)
    - [Indexed Access Types](#indexed-access-types)
    - [Utility Types](#utility-types)
      - [Awaited\<T\>](#awaitedt)
      - [Partial\<T\>](#partialt)
      - [Required\<T\>](#requiredt)
      - [Readonly\<T\>](#readonlyt)
      - [Record\<K, T\>](#recordk-t)
      - [Pick\<T, K\>](#pickt-k)
      - [Omit\<T, K\>](#omitt-k)
      - [Exclude\<T, U\>](#excludet-u)
      - [Extract\<T, U\>](#extractt-u)
      - [NonNullable\<T\>](#nonnullablet)
      - [Parameters\<T\>](#parameterst)
      - [ConstructorParameters\<T\>](#constructorparameterst)
      - [ReturnType\<T\>](#returntypet)
      - [InstanceType\<T\>](#instancetypet)
      - [ThisParameterType\<T\>](#thisparametertypet)
      - [OmitThisParameter\<T\>](#omitthisparametert)
      - [ThisType\<T\>](#thistypet)
      - [Uppercase\<T\>](#uppercaset)
      - [Lowercase\<T\>](#lowercaset)
      - [Capitalize\<T\>](#capitalizet)
      - [Uncapitalize\<T\>](#uncapitalizet)
      - [NoInfer\<T\>](#noinfert)
  - [Overige](#overige)
    - [Fouten en Exception Handling](#fouten-en-exception-handling)
    - [Mixin classes](#mixin-classes)
    - [Asynchrone Taalfuncties](#asynchrone-taalfuncties)
    - [Iterators en Generators](#iterators-en-generators)
    - [TsDocs JSDoc Referentie](#tsdocs-jsdoc-referentie)
    - [@types](#types-1)
    - [JSX](#jsx-1)
    - [ES6 Modules](#es6-modules)
    - [ES7 Exponentiation Operator](#es7-exponentiation-operator)
    - [Het for-await-of Statement](#het-for-await-of-statement)
    - [Nieuwe target meta-property](#nieuwe-target-meta-property)
    - [Dynamic Import Expressies](#dynamic-import-expressies)
    - ["tsc –watch"](#tsc-watch)
    - [Non-null Assertion Operator](#non-null-assertion-operator)
    - [Defaulted declaraties](#defaulted-declaraties)
    - [Optional Chaining](#optional-chaining)
    - [Nullish coalescing operator](#nullish-coalescing-operator)
    - [Template Literal Types](#template-literal-types)
    - [Function overloading](#function-overloading)
    - [Recursieve Types](#recursieve-types)
    - [Recursieve Conditional Types](#recursieve-conditional-types)
    - [ECMAScript Module Ondersteuning in Node](#ecmascript-module-ondersteuning-in-node)
    - [Assertion Functions](#assertion-functions)
    - [Variadic Tuple Types](#variadic-tuple-types)
    - [Boxed types](#boxed-types)
    - [Covariantie en Contravariantie in TypeScript](#covariantie-en-contravariantie-in-typescript)
      - [Optionele Variantie-annotaties voor Type Parameters](#optionele-variantie-annotaties-voor-type-parameters)
    - [Template String Pattern Index Signatures](#template-string-pattern-index-signatures)
    - [De satisfies Operator](#de-satisfies-operator)
    - [Type-Only Imports en Export](#type-only-imports-en-export)
    - [using declaratie en Explicit Resource Management](#using-declaratie-en-explicit-resource-management)
      - [await using declaratie](#await-using-declaratie)
    - [Import Attributes](#import-attributes)
<!-- markdownlint-enable MD004 -->

## Inleiding

Welkom bij Het Beknopte TypeScript Boek! Deze gids voorziet je van essentiële kennis en praktische vaardigheden voor effectieve TypeScript-ontwikkeling. Ontdek kernconcepten en technieken om schone, robuuste code te schrijven. Of je nu een beginner bent of een ervaren ontwikkelaar, dit boek dient als zowel een uitgebreide gids als een handig naslagwerk voor het benutten van de kracht van TypeScript in je projecten.

Dit boek behandelt TypeScript 5.2.

## Over de auteur

Simone Poggiali is een ervaren Staff Engineer met een passie voor het schrijven van professionele code sinds de jaren 90. Gedurende zijn internationale carrière heeft hij bijgedragen aan tal van projecten voor een breed scala aan klanten, van startups tot grote organisaties. Gerenommeerde bedrijven zoals HelloFresh, Siemens, O2, Leroy Merlin en Snowplow hebben geprofiteerd van zijn expertise en toewijding.

Je kunt Simone Poggiali bereiken op de volgende platforms:

* LinkedIn: [https://www.linkedin.com/in/simone-poggiali](https://www.linkedin.com/in/simone-poggiali)
* GitHub: [https://github.com/gibbok](https://github.com/gibbok)
* X.com: [https://x.com/gibbok_coding](https://x.com/gibbok_coding)
* E-mail: gibbok.coding📧gmail.com

## Introductie tot TypeScript

### Wat is TypeScript?

TypeScript is een sterk getypeerde programmeertaal die voortbouwt op JavaScript. Het werd oorspronkelijk ontworpen door Anders Hejlsberg in 2012 en wordt momenteel ontwikkeld en onderhouden door Microsoft als een open-source project.

TypeScript compileert naar JavaScript en kan worden uitgevoerd in elke JavaScript-runtime (bijv. een browser of server-side Node.js).

TypeScript ondersteunt meerdere programmeerparadigma's, zoals functioneel, generiek, imperatief en objectgeoriënteerd. TypeScript is noch een geïnterpreteerde, noch een gecompileerde taal in de traditionele zin.

### Waarom TypeScript?

TypeScript is een sterk getypeerde taal die helpt bij het voorkomen van veelvoorkomende programmeerfouten en het vermijden van bepaalde soorten runtime-fouten voordat het programma wordt uitgevoerd.

Een sterk getypeerde taal stelt de ontwikkelaar in staat om verschillende programmabeperkingen en -gedragingen te specificeren in de datatypedefinities, wat het gemakkelijker maakt om de correctheid van de software te verifiëren en defecten te voorkomen. Dit is vooral waardevol in grootschalige applicaties.

Enkele voordelen van TypeScript:

* Statische typering, optioneel sterk getypeerd
* Type Inference (Type-afleiding)
* Toegang tot ES6- en ES7-functies
* Cross-platform en cross-browser compatibiliteit
* Tooling-ondersteuning met IntelliSense

### TypeScript en JavaScript

TypeScript wordt geschreven in `.ts` of `.tsx` bestanden, terwijl JavaScript-bestanden worden geschreven in `.js` of `.jsx`.

Bestanden met de extensie `.tsx` of `.jsx` kunnen JavaScript Syntax Extension (JSX) bevatten, wat in React wordt gebruikt voor UI-ontwikkeling.

TypeScript is een getypeerde superset van JavaScript (ECMAScript 2015) qua syntaxis. Alle JavaScript-code is geldige TypeScript-code, maar het omgekeerde is niet altijd waar.

Beschouw bijvoorbeeld een functie in een JavaScript-bestand met de extensie `.js`, zoals de volgende:

<!-- skip -->
```typescript
const sum = (a, b) => a + b;
```

De functie kan worden geconverteerd en gebruikt in TypeScript door de bestandsextensie te wijzigen naar `.ts`. Als dezelfde functie echter wordt geannoteerd met TypeScript-types, kan deze zonder compilatie niet worden uitgevoerd in een JavaScript-runtime. De volgende TypeScript-code zal een syntaxfout veroorzaken als deze niet wordt gecompileerd:

<!-- skip -->
```typescript
const sum = (a: number, b: number): number => a + b;
```

TypeScript is ontworpen om mogelijke uitzonderingen die tijdens runtime kunnen optreden te detecteren tijdens de compilatie, door de ontwikkelaar de intentie te laten definiëren met type-annotaties. Daarnaast kan TypeScript ook problemen opvangen als er geen type-annotatie is opgegeven. Het volgende codefragment specificeert bijvoorbeeld geen TypeScript-types:

<!-- skip -->
```typescript
const items = [{ x: 1 }, { x: 2 }];
const result = items.filter(item => item.y);
```

In dit geval detecteert TypeScript een fout en rapporteert:

```text
Property 'y' does not exist on type '{ x: number; }'.
```

Het typesysteem van TypeScript is grotendeels beïnvloed door het runtime-gedrag van JavaScript. De optellingsoperator (+), die in JavaScript ofwel string-concatenatie of numerieke optelling kan uitvoeren, is bijvoorbeeld op dezelfde manier gemodelleerd in TypeScript:

```typescript
const result = '1' + 1; // Resultaat is van type string
```

Het team achter TypeScript heeft de bewuste beslissing genomen om ongebruikelijk gebruik van JavaScript als fouten te markeren. Beschouw bijvoorbeeld de volgende geldige JavaScript-code:

<!-- skip -->
```typescript
const result = 1 + true; // In JavaScript is het resultaat gelijk aan 2
```

TypeScript geeft echter een foutmelding:

```text
Operator '+' cannot be applied to types 'number' and 'boolean'.
```

Deze fout treedt op omdat TypeScript strikt type-compatibiliteit afdwingt, en in dit geval identificeert het een ongeldige bewerking tussen een getal en een boolean.

### TypeScript Codegeneratie

De TypeScript-compiler heeft twee hoofdtaken: controleren op typefouten en compileren naar JavaScript. Deze twee processen staan los van elkaar. Types hebben geen invloed op de uitvoering van de code in een JavaScript-runtime, omdat ze volledig worden verwijderd tijdens de compilatie. TypeScript kan nog steeds JavaScript uitvoeren, zelfs als er typefouten aanwezig zijn.
Hier is een voorbeeld van TypeScript-code met een typefout:

<!-- skip -->
```typescript
const add = (a: number, b: number): number => a + b;
const result = add('x', 'y'); // Argument of type 'string' is not assignable to parameter of type 'number'.
```

Het kan echter nog steeds uitvoerbare JavaScript-output produceren:

<!-- skip -->
```typescript
'use strict';
const add = (a, b) => a + b;
const result = add('x', 'y'); // xy
```

Het is niet mogelijk om TypeScript-types te controleren tijdens runtime. Bijvoorbeeld:

<!-- skip -->
```typescript
interface Animal {
    name: string;
}
interface Dog extends Animal {
    bark: () => void;
}
interface Cat extends Animal {
    meow: () => void;
}
const makeNoise = (animal: Animal) => {
    if (animal instanceof Dog) {
        // 'Dog' only refers to a type, but is being used as a value here.
        // ...
    }
};
```

Omdat de types na compilatie zijn gewist, is er geen manier om deze code in JavaScript uit te voeren. Om types tijdens runtime te herkennen, moeten we een ander mechanisme gebruiken. TypeScript biedt verschillende opties, waarvan een veelvoorkomende de "tagged union" is. Bijvoorbeeld:

```typescript
interface Dog {
    kind: 'dog'; // Tagged union
    bark: () => void;
}
interface Cat {
    kind: 'cat'; // Tagged union
    meow: () => void;
}
type Animal = Dog | Cat;

const makeNoise = (animal: Animal) => {
    if (animal.kind === 'dog') {
        animal.bark();
    } else {
        animal.meow();
    }
};

const dog: Dog = {
    kind: 'dog',
    bark: () => console.log('bark'),
};
makeNoise(dog);
```

De eigenschap "kind" is een waarde die tijdens runtime kan worden gebruikt om objecten in JavaScript te onderscheiden.

Het is ook mogelijk dat een waarde tijdens runtime een ander type heeft dan aangegeven in de typedeclaratie. Bijvoorbeeld als de ontwikkelaar een API-type verkeerd heeft geïnterpreteerd en onjuist heeft geannoteerd.

TypeScript is een superset van JavaScript, dus het trefwoord "class" kan zowel als type als waarde tijdens runtime worden gebruikt.

```typescript
class Animal {
    constructor(public name: string) {}
}
class Dog extends Animal {
    constructor(
        public name: string,
        public bark: () => void
    ) {
        super(name);
    }
}
class Cat extends Animal {
    constructor(
        public name: string,
        public meow: () => void
    ) {
        super(name);
    }
}
type Mammal = Dog | Cat;

const makeNoise = (mammal: Mammal) => {
    if (mammal instanceof Dog) {
        mammal.bark();
    } else {
        mammal.meow();
    }
};

const dog = new Dog('Fido', () => console.log('bark'));
makeNoise(dog);
```

In JavaScript heeft een "class" een "prototype" eigenschap, en de "instanceof" operator kan worden gebruikt om te testen of de prototype-eigenschap van een constructor ergens in de prototype-chain van een object voorkomt.

TypeScript heeft geen invloed op de runtime-prestaties, omdat alle types worden verwijderd. TypeScript introduceert echter wel wat overhead tijdens de bouwtijd (build time).

### Modern JavaScript Nu (Downleveling)

TypeScript kan code compileren naar elke uitgebrachte versie van JavaScript sinds ECMAScript 3 (1999). Dit betekent dat TypeScript code van de nieuwste JavaScript-functies kan transpileren naar oudere versies, een proces dat bekend staat als Downleveling. Dit maakt het gebruik van modern JavaScript mogelijk met behoud van maximale compatibiliteit met oudere runtime-omgevingen.

Het is belangrijk op te merken dat TypeScript tijdens het transpileren naar een oudere versie van JavaScript code kan genereren die een prestatie-overhead kan veroorzaken in vergelijking met eigen implementaties.

Hier zijn enkele moderne JavaScript-functies die in TypeScript kunnen worden gebruikt:

* ECMAScript-modules in plaats van AMD-stijl "define" callbacks of CommonJS "require" statements.
* Classes in plaats van prototypes.
* Variabeledeclaratie met "let" of "const" in plaats van "var".
* "for-of" loop of ".forEach" in plaats van de traditionele "for" loop.
* Arrow functions in plaats van function expressions.
* Destructuring assignment (Destructurerende toewijzing).
* Kortere notatie voor eigenschaps-/methodenamen en berekende eigenschapsnamen.
* Standaard functieparameters.

Door gebruik te maken van deze moderne JavaScript-functies kunnen ontwikkelaars expressievere en beknoptere code schrijven in TypeScript.

## Aan de slag met TypeScript

### Installatie

Visual Studio Code biedt uitstekende ondersteuning voor de taal TypeScript, maar bevat niet de TypeScript-compiler. Om de TypeScript-compiler te installeren, kun je een pakketbeheerder zoals npm of yarn gebruiken:

```shell
npm install typescript --save-dev
```

of

```shell
yarn add typescript --dev
```

Zorg ervoor dat je het gegenereerde lock-bestand commit om te garanderen dat elk teamlid dezelfde versie van TypeScript gebruikt.

Om de TypeScript-compiler uit te voeren, kun je de volgende commando's gebruiken:

```shell
npx tsc
```

of

```shell
yarn tsc
```

Het wordt aanbevolen om TypeScript project-breed te installeren in plaats van globaal, omdat dit een voorspelbaarder bouwproces oplevert. Voor eenmalige gelegenheden kun je echter het volgende commando gebruiken:

```shell
npx tsc
```

Of het globaal installeren:

```shell
npm install -g typescript
```

Als je Microsoft Visual Studio gebruikt, kun je TypeScript verkrijgen als een pakket in NuGet voor je MSBuild-projecten. Voer in de NuGet Package Manager Console het volgende commando uit:

```shell
Install-Package Microsoft.TypeScript.MSBuild
```

Tijdens de TypeScript-installatie worden twee uitvoerbare bestanden geïnstalleerd: "tsc" als de TypeScript-compiler en "tsserver" als de TypeScript standalone server. De standalone server bevat de compiler en taaldiensten die door editors en IDE's kunnen worden gebruikt om intelligente code-aanvulling te bieden.

Daarnaast zijn er verschillende TypeScript-compatibele transpilers beschikbaar, zoals Babel (via een plugin) of swc. Deze transpilers kunnen worden gebruikt om TypeScript-code om te zetten naar andere doeltalen of versies.

### Configuratie

TypeScript kan worden geconfigureerd met behulp van de tsc CLI-opties of door gebruik te maken van een speciaal configuratiebestand genaamd `tsconfig.json`, dat in de root van het project wordt geplaatst.

Om een `tsconfig.json` bestand te genereren dat vooraf is ingevuld met aanbevolen instellingen, kun je het volgende commando gebruiken:

```shell
tsc --init
```

Wanneer het `tsc` commando lokaal wordt uitgevoerd, zal TypeScript de code compileren met de configuratie die is gespecificeerd in het dichtstbijzijnde `tsconfig.json` bestand.

Hier zijn enkele voorbeelden van CLI-commando's die met de standaardinstellingen worden uitgevoerd:

```shell
tsc main.ts // Compileer een specifiek bestand (main.ts) naar JavaScript
tsc src/*.ts // Compileer alle .ts bestanden onder de 'src' map naar JavaScript
tsc app.ts util.ts --outfile index.js // Compileer twee TypeScript-bestanden (app.ts en util.ts) naar één enkel JavaScript-bestand (index.js)
```

### TypeScript Configuratiebestand

Een `tsconfig.json` bestand wordt gebruikt om de TypeScript Compiler (tsc) te configureren. Gewoonlijk wordt het toegevoegd aan de root van het project, samen met het `package.json` bestand.

Opmerkingen:

* `tsconfig.json` accepteert commentaar, zelfs al is het in JSON-formaat.
* Het is raadzaam om dit configuratiebestand te gebruiken in plaats van de opdrachtregelopties.

Op de volgende link vind je de volledige documentatie en het schema:

[https://www.typescriptlang.org/tsconfig](https://www.typescriptlang.org/tsconfig)

[https://www.typescriptlang.org/tsconfig/](https://www.typescriptlang.org/tsconfig/)

Hieronder volgt een lijst van veelvoorkomende en nuttige configuraties:

#### target

De eigenschap "target" wordt gebruikt om aan te geven naar welke versie van JavaScript ECMAScript je TypeScript moet emitteren/compileren. Voor moderne browsers is ES6 een goede optie; voor oudere browsers wordt ES5 aanbevolen.

#### lib

De eigenschap "lib" wordt gebruikt om aan te geven welke bibliotheekbestanden moeten worden opgenomen tijdens de compilatie. TypeScript bevat automatisch API's voor functies die zijn gespecificeerd in de eigenschap "target", maar het is mogelijk om specifieke bibliotheken weg te laten of te kiezen voor specifieke behoeften. Als je bijvoorbeeld aan een serverproject werkt, zou je de "DOM"-bibliotheek kunnen uitsluiten, die alleen nuttig is in een browseromgeving.

#### strict

De eigenschap "strict" maakt sterkere garanties mogelijk en verbetert de typeveiligheid. Het is raadzaam om deze eigenschap altijd op te nemen in het `tsconfig.json` bestand van je project. Door de eigenschap "strict" in te schakelen, kan TypeScript:

* Code genereren met "use strict" voor elk bronbestand.
* "null" en "undefined" meenemen in het type-checking proces.
* Het gebruik van het type "any" uitschakelen wanneer er geen type-annotaties aanwezig zijn.
* Een foutmelding geven bij het gebruik van de "this"-expressie wanneer deze anders het type "any" zou impliceren.

#### module

De eigenschap "module" stelt het modulesysteem in dat wordt ondersteund voor het gecompileerde programma. Tijdens runtime wordt een module-loader gebruikt om afhankelijkheden te lokaliseren en uit te voeren op basis van het gespecificeerde modulesysteem.

De meest voorkomende module-loaders die in JavaScript worden gebruikt zijn Node.js CommonJS voor server-side applicaties en RequireJS voor AMD-modules in browser-gebaseerde webapplicaties. TypeScript kan code genereren voor verschillende modulesystemen, waaronder UMD, System, ESNext, ES2015/ES6 en ES2020.

Opmerking: Het modulesysteem moet worden gekozen op basis van de doelomgeving en het module-laadmechanisme dat beschikbaar is in die omgeving.

#### moduleResolution

De eigenschap "moduleResolution" specificeert de strategie voor module-resolutie. Gebruik "node" voor moderne TypeScript-code; de "classic" strategie wordt alleen gebruikt voor oude versies van TypeScript (vóór 1.6).

#### esModuleInterop

De eigenschap "esModuleInterop" maakt het mogelijk om de standaard export (default import) te gebruiken van CommonJS-modules die niet zijn geëxporteerd met de eigenschap "default". Deze eigenschap biedt een shim om compatibiliteit in de gegenereerde JavaScript te garanderen. Na het inschakelen van deze optie kunnen we `import MyLibrary from "my-library"` gebruiken in plaats van `import * as MyLibrary from "my-library"`.

#### jsx

De eigenschap "jsx" is alleen van toepassing op .tsx-bestanden die in ReactJS worden gebruikt en bepaalt hoe JSX-constructies naar JavaScript worden gecompileerd. Een veelvoorkomende optie is "preserve", die compileert naar een .jsx-bestand waarbij de JSX ongewijzigd blijft, zodat deze kan worden doorgegeven aan andere tools zoals Babel voor verdere transformaties.

#### skipLibCheck

De eigenschap "skipLibCheck" voorkomt dat TypeScript de volledige geïmporteerde pakketten van derden controleert. Deze eigenschap verkort de compilatietijd van een project. TypeScript zal je code nog steeds controleren aan de hand van de typedefinities die door deze pakketten worden geleverd.

#### files

De eigenschap "files" geeft de compiler een lijst van bestanden die altijd in het programma moeten worden opgenomen.

#### include

<!-- markdownlint-disable MD049 -->
De eigenschap "include" geeft de compiler een lijst van bestanden die we willen opnemen. Deze eigenschap staat glob-achtige patronen toe, zoals `**/*` voor elke submap, `*` voor elke bestandsnaam en `?` voor optionele tekens.
<!-- markdownlint-enable MD049 -->

#### exclude

De eigenschap "exclude" geeft de compiler een lijst van bestanden die niet in de compilatie moeten worden opgenomen. Dit kunnen bestanden zijn zoals "node_modules" of testbestanden.
Opmerking: `tsconfig.json` staat commentaar toe.

### importHelpers

TypeScript gebruikt helpercode bij het genereren van code voor bepaalde geavanceerde of gedownlevelde JavaScript-functies. Standaard worden deze helpers gedupliceerd in de bestanden die ze gebruiken. De optie `importHelpers` importeert deze helpers in plaats daarvan uit de `tslib` module, wat de JavaScript-output efficiënter maakt.

### Advies voor migratie naar TypeScript

Voor grote projecten wordt een geleidelijke overgang aanbevolen, waarbij TypeScript- en JavaScript-code in eerste instantie naast elkaar bestaan. Alleen kleine projecten kunnen in één keer naar TypeScript worden gemigreerd.

De eerste stap van deze overgang is het introduceren van TypeScript in het build-chain proces. Dit kan worden gedaan door de compileroptie "allowJs" te gebruiken, die toestaat dat .ts en .tsx bestanden naast bestaande JavaScript-bestanden bestaan. Omdat TypeScript terugvalt op een type van "any" voor een variabele wanneer het het type niet kan afleiden uit JavaScript-bestanden, wordt aanbevolen om "noImplicitAny" uit te schakelen in je compileropties aan het begin van de migratie.

De tweede stap is ervoor te zorgen dat je JavaScript-tests werken naast TypeScript-bestanden, zodat je tests kunt uitvoeren terwijl je elke module converteert. Als je Jest gebruikt, overweeg dan het gebruik van `ts-jest`, waarmee je TypeScript-projecten met Jest kunt testen.

De derde stap is het opnemen van typedeclaraties voor bibliotheken van derden in je project. Deze declaraties kunnen ofwel gebundeld worden gevonden of op DefinitelyTyped. Je kunt ze zoeken via [https://www.typescriptlang.org/dt/search](https://www.typescriptlang.org/dt/search) en ze installeren met:

```shell
npm install --save-dev @types/pakketnaam
```

of

```shell
yarn add --dev @types/pakketnaam
```

De vierde stap is om module voor module te migreren met een bottom-up benadering, waarbij je de afhankelijkheidsgraaf (Dependency Graph) volgt beginnend bij de bladeren (leaves). Het idee is om te beginnen met het converteren van modules die niet afhankelijk zijn van andere modules. Om de afhankelijkheidsgrafen te visualiseren, kun je de tool "madge" gebruiken.

Goede kandidaten voor deze eerste conversies zijn utility-functies en code gerelateerd aan externe API's of specificaties. Het is mogelijk om automatisch TypeScript-typedefinities te genereren uit Swagger-contracten, GraphQL of JSON-schema's om in je project op te nemen.

Wanneer er geen officiële specificaties of schema's beschikbaar zijn, kun je types genereren uit ruwe data, zoals JSON die door een server wordt geretourneerd. Het wordt echter aanbevolen om types te genereren uit specificaties in plaats van data om het missen van randgevallen te voorkomen.

Onthoud je tijdens de migratie van het herstructureren (refactoring) van code en focus je alleen op het toevoegen van types aan je modules.

De vijfde stap is het inschakelen van "noImplicitAny", wat zal afdwingen dat alle types bekend en gedefinieerd zijn, wat een betere TypeScript-ervaring voor je project oplevert.

Tijdens de migratie kun je de `@ts-check` directive gebruiken, die TypeScript-typecontrole inschakelt in een JavaScript-bestand. Deze directive biedt een lossere versie van typecontrole en kan in het begin worden gebruikt om problemen in JavaScript-bestanden te identificeren. Wanneer `@ts-check` in een bestand is opgenomen, zal TypeScript proberen definities af te leiden met behulp van JSDoc-stijl commentaar. Overweeg echter om JSDoc-annotaties alleen in een zeer vroeg stadium van de migratie te gebruiken.

Overweeg om de standaardwaarde van `noEmitOnError` in je `tsconfig.json` op false te laten staan. Hierdoor kun je JavaScript-broncode genereren, zelfs als er fouten worden gerapporteerd.

## Het typesysteem verkennen

### De TypeScript Language Service

De TypeScript Language Service, ook bekend als tsserver, biedt verschillende functies zoals foutrapportage, diagnostiek, compile-on-save, hernoemen, ga naar definitie, voltooiingslijsten, hulp bij signaturen en meer. Het wordt voornamelijk gebruikt door geïntegreerde ontwikkelomgevingen (IDE's) om IntelliSense-ondersteuning te bieden. Het integreert naadloos met Visual Studio Code en wordt gebruikt door tools zoals Conquer of Completion (Coc).

Ontwikkelaars kunnen gebruikmaken van een speciale API en hun eigen aangepaste language service plugins maken om de TypeScript-bewerkingservaring te verbeteren. Dit kan bijzonder nuttig zijn voor het implementeren van speciale linting-functies of het inschakelen van auto-complete voor een aangepaste templatingtaal.

<!-- markdownlint-disable MD044 -->
Een voorbeeld van een echte aangepaste plugin is "typescript-styled-plugin", die syntaxfoutrapportage en IntelliSense-ondersteuning biedt voor CSS-eigenschappen in styled-components.
<!-- markdownlint-enable MD044 -->

Voor meer informatie en snelstartgidsen kun je de officiële TypeScript Wiki op GitHub raadplegen: [https://github.com/microsoft/TypeScript/wiki/](https://github.com/microsoft/TypeScript/wiki/)

### Structurele Typering

TypeScript is gebaseerd on een structureel typesysteem. Dit betekent dat de compatibiliteit en gelijkwaardigheid van types worden bepaald door de feitelijke structuur of definitie van het type, in plaats van de naam of de plaats van declaratie, zoals in nominatieve typesystemen zoals C# of C++.

Het structurele typesysteem van TypeScript is ontworpen op basis van hoe het dynamische duck-typing systeem van JavaScript werkt tijdens runtime.

Het volgende voorbeeld is geldige TypeScript-code. Zoals je kunt zien, hebben "X" en "Y" hetzelfde lid "a", ook al hebben ze verschillende declaratienamen. De types worden bepaald door hun structuren, en in dit geval, aangezien de structuren hetzelfde zijn, zijn ze compatibel en geldig.

```typescript
type X = {
    a: string;
};
type Y = {
    a: string;
};
const x: X = { a: 'a' };
const y: Y = x; // Geldig
```

### Fundamentele vergelijkingsregels van TypeScript

Het vergelijkingsproces van TypeScript is recursief en wordt uitgevoerd op types die op elk niveau genest zijn.

Een type "X" is compatibel met "Y" als "Y" ten minste dezelfde leden heeft als "X".

```typescript
type X = {
    a: string;
};
const y = { a: 'A', b: 'B' }; // Geldig, omdat het ten minste dezelfde leden heeft als X
const r: X = y;
```

Functieparameters worden vergeleken op basis van types, niet op basis van hun namen:

```typescript
type X = (a: number) => void;
type Y = (a: number) => void;
let x: X = (j: number) => undefined;
let y: Y = (k: number) => undefined;
y = x; // Geldig
x = y; // Geldig
```

Return-types van functies moeten hetzelfde zijn:

<!-- skip -->
```typescript
type X = (a: number) => undefined;
type Y = (a: number) => number;
let x: X = (a: number) => undefined;
let y: Y = (a: number) => 1;
y = x; // Ongeldig
x = y; // Ongeldig
```

Het return-type van een bronfunctie moet een subtype zijn van het return-type van een doelfunctie:

<!-- skip -->
```typescript
let x = () => ({ a: 'A' });
let y = () => ({ a: 'A', b: 'B' });
x = y; // Geldig
y = x; // Ongeldig: lid b ontbreekt
```

Het negeren van functieparameters is toegestaan, omdat dit een veelvoorkomende praktijk is in JavaScript, bijvoorbeeld bij het gebruik van `Array.prototype.map()`:

```typescript
[1, 2, 3].map((element, _index, _array) => element + 'x');
```

Daarom zijn de volgende typedeclaraties volledig geldig:

```typescript
type X = (a: number) => undefined;
type Y = (a: number, b: number) => undefined;
let x: X = (a: number) => undefined;
let y: Y = (a: number) => undefined; // Parameter b ontbreekt
y = x; // Geldig
```

Eventuele extra optionele parameters van het brontype zijn geldig:

```typescript
type X = (a: number, b?: number, c?: number) => undefined;
type Y = (a: number) => undefined;
let x: X = a => undefined;
let y: Y = a => undefined;
y = x; // Geldig
x = y; // Geldig
```

Eventuele optionele parameters van het doeltype zonder overeenkomstige parameters in het brontype zijn geldig en geen fout:

```typescript
type X = (a: number) => undefined;
type Y = (a: number, b?: number) => undefined;
let x: X = a => undefined;
let y: Y = a => undefined;
y = x; // Geldig
x = y; // Geldig
```

De rest-parameter wordt behandeld als een oneindige reeks optionele parameters:

```typescript
type X = (a: number, ...rest: number[]) => undefined;
let x: X = a => undefined; // Geldig
```

Functies met overloads zijn geldig als de overload-signatuur compatibel is met de implementatie-signatuur:

<!-- skip -->
```typescript
function x(a: string): void;
function x(a: string, b: number): void;
function x(a: string, b?: number): void {
    console.log(a, b);
}
x('a'); // Geldig
x('a', 1); // Geldig

function y(a: string): void; // Ongeldig, niet compatibel met implementatie-signatuur
function y(a: string, b: number): void;
function y(a: string, b: number): void {
    console.log(a, b);
}
y('a');
y('a', 1);
```

Vergelijking van functieparameters slaagt als de bron- en doelparameters toewijsbaar zijn aan supertypes of subtypes (bivariantie).

```typescript
// Supertype
class X {
    a: string;
    constructor(value: string) {
        this.a = value;
    }
}
// Subtype
class Y extends X {}
// Subtype
class Z extends X {}

type GetA = (x: X) => string;
const getA: GetA = x => x.a;

// Bivariantie accepteert supertypes
console.log(getA(new X('x'))); // Geldig
console.log(getA(new Y('Y'))); // Geldig
console.log(getA(new Z('z'))); // Geldig
```

Enums zijn vergelijkbaar en geldig met getallen en vice versa, maar het vergelijken van Enum-waarden van verschillende Enum-types is ongeldig.

<!-- skip -->
```typescript
enum X {
    A,
    B,
}
enum Y {
    A,
    B,
    C,
}
const xa: number = X.A; // Geldig
const ya: Y = 0; // Geldig
X.A === Y.A; // Ongeldig
```

Instanties van een class zijn onderworpen aan een compatibiliteitscontrole voor hun private en protected leden:

<!-- skip -->
```typescript
class X {
    public a: string;
    constructor(value: string) {
        this.a = value;
    }
}

class Y {
    private a: string;
    constructor(value: string) {
        this.a = value;
    }
}

let x: X = new Y('y'); // Ongeldig
```

De vergelijkingscontrole houdt geen rekening met verschillende overervingshiërarchieën, bijvoorbeeld:

```typescript
class X {
    public a: string;
    constructor(value: string) {
        this.a = value;
    }
}
class Y extends X {
    public a: string;
    constructor(value: string) {
        super(value);
        this.a = value;
    }
}
class Z {
    public a: string;
    constructor(value: string) {
        this.a = value;
    }
}
let x: X = new X('x');
let y: Y = new Y('y');
let z: Z = new Z('z');
x === y; // Geldig
x === z; // Geldig, zelfs als z uit een andere overervingshiërarchie komt
```

Generics worden vergeleken op basis van hun structuren na toepassing van de generieke parameter; alleen het eindresultaat wordt vergeleken als een niet-generiek type.

<!-- skip -->
```typescript
interface X<T> {
    a: T;
}
let x: X<number> = { a: 1 };
let y: X<string> = { a: 'a' };
x === y; // Ongeldig omdat het type-argument wordt gebruikt in de uiteindelijke structuur
```

```typescript
interface X<T> {}
const x: X<number> = 1;
const y: X<string> = 'a';
x === y; // Geldig omdat het type-argument niet wordt gebruikt in de uiteindelijke structuur
```

Wanneer generics geen opgegeven type-argument hebben, worden alle niet-gespecificeerde argumenten behandeld als types met "any":

```typescript
type X = <T>(x: T) => T;
type Y = <K>(y: K) => K;
let x: X = x => x;
let y: Y = y => y;
x = y; // Geldig
```

Onthoud:

<!-- skip -->
```typescript
let a: number = 1;
let b: number = 2;
a = b; // Geldig, alles is toewijsbaar aan zichzelf

let c: any;
c = 1; // Geldig, alle types zijn toewijsbaar aan any

let d: unknown;
d = 1; // Geldig, alle types zijn toewijsbaar aan unknown

let e: unknown;
let e1: unknown = e; // Geldig, unknown is alleen toewijsbaar aan zichzelf en any
let e2: any = e; // Geldig
let e3: number = e; // Ongeldig

let f: never;
f = 1; // Ongeldig, niets is toewijsbaar aan never

let g: void;
let g1: any;
g = 1; // Ongeldig, void is aan niets toewijsbaar, behalve aan any
g = g1; // Geldig
```

Houd er rekening mee dat wanneer "strictNullChecks" is ingeschakeld, "null" en "undefined" vergelijkbaar worden behandeld als "void"; anders zijn ze vergelijkbaar met "never".

### Types als Verzamelingen

In TypeScript is een type een verzameling mogelijke waarden. Deze verzameling wordt ook wel het domein van het type genoemd. Elke waarde van een type kan worden gezien als een element in een verzameling. Een type stelt de beperkingen vast waaraan elk element in de verzameling moet voldoen om als lid van die verzameling te worden beschouwd.
De hoofdtaak van TypeScript is om te controleren en te verifiëren of de ene verzameling een deelverzameling (subset) is van de andere.

TypeScript ondersteunt verschillende soorten verzamelingen:

| Verzamelingsterm   | TypeScript                      | Opmerkingen                                                                                                        |
| ------------------ | ------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Lege verzameling   | never                           | "never" bevat niets behalve zichzelf                                                                               |
| Enkelvoudige verz. | undefined / null / literal type |                                                                                                                    |
| Eindige verz.      | boolean / union                 |                                                                                                                    |
| Oneindige verz.    | string / number / object        |                                                                                                                    |
| Universele verz.   | any / unknown                   | Elk element is lid van "any" en elke verzameling is er een deelverzameling van / "unknown" is de veilige tegenhanger van "any" |

Hier zijn enkele voorbeelden:

| TypeScript            | Verzamelingsterm       | Voorbeeld                                                                       |
| --------------------- | ---------------------- | ------------------------------------------------------------------------------- |
| never                 | ∅ (lege verzameling)   | const x: never = 'x'; // Fout: Type 'string' is niet toewijsbaar aan type 'never' |
|                       |                        |
| Literal type          | Enkelvoudige verz.     | type X = 'X';                                                                   |
|                       |                        | type Y = 7;                                                                     |
|                       |                        |
| Waarde toewijsbaar aan T | Waarde ∈ T (lid van)  | type XY = 'X' \| 'Y';                                                           |
|                       |                        | const x: XY = 'X';                                                              |
|                       |                        |
| T1 toewijsbaar aan T2 | T1 ⊆ T2 (subset van)   | type XY = 'X' \| 'Y';                                                           |
|                       |                        | const x: XY = 'X';                                                              |
|                       |                        | const j: XY = 'J'; // Type '"J"' is niet toewijsbaar aan type 'XY'.                |
|                       |                        |                                                                                 |
| T1 extends T2         | T1 ⊆ T2 (subset van)   | type X = 'X' extends string ? true : false;                                     |
|                       |                        |
| T1 \| T2              | T1 ∪ T2 (unie)         | type XY = 'X' \| 'Y';                                                           |
|                       |                        | type JK = 1 \| 2;                                                               |
|                       |                        |
| T1 & T2               | T1 ∩ T2 (doorsnede)    | type X = { a: string }                                                          |
|                       |                        | type Y = { b: string }                                                          |
|                       |                        | type XY = X & Y                                                                 |
|                       |                        | const x: XY = { a: 'a', b: 'b' }                                                |
|                       |                        |
| unknown               | Universele verzameling | const x: unknown = 1                                                            |

Een unie (T1 | T2) creëert een bredere verzameling (beide):

```typescript
type X = {
    a: string;
};
type Y = {
    b: string;
};
type XY = X | Y;
const r: XY = { a: 'a', b: 'x' }; // Geldig
```

Een doorsnede (intersection, T1 & T2) creëert een nauwere verzameling (alleen gedeeld):

<!-- skip -->
```typescript
type X = {
    a: string;
};
type Y = {
    a: string;
    b: string;
};
type XY = X & Y;
const r: XY = { a: 'a' }; // Ongeldig
const j: XY = { a: 'a', b: 'b' }; // Geldig
```

Het trefwoord `extends` kan in deze context worden beschouwd als "deelverzameling van". Het stelt een beperking (constraint) voor een type vast. Wanneer `extends` wordt gebruikt met een generic, wordt de generic gezien als een oneindige verzameling en wordt deze beperkt tot een specifiekere verzameling.
Houd er rekening mee dat `extends` niets te maken heeft met hiërarchie in de zin van OOP (dit concept bestaat niet in TypeScript).
TypeScript werkt met verzamelingen en heeft geen strikte hiërarchie; in feite kunnen twee types elkaar overlappen zonder dat de een een subtype is van de ander (TypeScript kijkt naar de structuur of vorm van de objecten).

```typescript
interface X {
    a: string;
}
interface Y extends X {
    b: string;
}
interface Z extends Y {
    c: string;
}
const z: Z = { a: 'a', b: 'b', c: 'c' };
interface X1 {
    a: string;
}
interface Y1 {
    a: string;
    b: string;
}
interface Z1 {
    a: string;
    b: string;
    c: string;
}
const z1: Z1 = { a: 'a', b: 'b', c: 'c' };

const r: Z1 = z; // Geldig
```

### Een type toewijzen: Typedeclaraties en Type-assertions

Een type kan op verschillende manieren worden toegewezen in TypeScript:

#### Typedeclaratie

In het volgende voorbeeld gebruiken we `x: X` (": Type") om een type voor de variabele x te declareren.

```typescript
type X = {
    a: string;
};

// Typedeclaratie
const x: X = {
    a: 'a',
};
```

Als de variabele niet in het opgegeven formaat is, zal TypeScript een fout rapporteren. Bijvoorbeeld:

<!-- skip -->
```typescript
type X = {
    a: string;
};

const x: X = {
    a: 'a',
    b: 'b', // Fout: Object literal mag alleen bekende eigenschappen specificeren
};
```

#### Type-assertion

Het is mogelijk om een bewering (assertion) toe te voegen met behulp van het trefwoord `as`. Dit vertelt de compiler dat de ontwikkelaar meer informatie heeft over een type en onderdrukt eventuele foutmeldingen.

Bijvoorbeeld:

```typescript
type X = {
    a: string;
};
const x = {
    a: 'a',
    b: 'b',
} as X;
```

In het bovenstaande voorbeeld wordt beweerd dat het object x het type X heeft met behulp van het trefwoord `as`. Dit informeert de TypeScript-compiler dat het object voldoet aan het gespecificeerde type, ook al heeft het een extra eigenschap b die niet in de typedefinitie voorkomt.

Type-assertions zijn nuttig in situaties waarin een specifiek type moet worden opgegeven, vooral bij het werken met de DOM. Bijvoorbeeld:

```typescript
const myInput = document.getElementById('my_input') as HTMLInputElement;
```

Hier wordt de type-assertion `as HTMLInputElement` gebruikt om TypeScript te vertellen dat het resultaat van `getElementById` behandeld moet worden als een `HTMLInputElement`.
Type-assertions kunnen ook worden gebruikt om keys te remap-pen, zoals in het onderstaande voorbeeld met template literals:

```typescript
type J<Type> = {
    [Property in keyof Type as `prefix_${string &
        Property}`]: () => Type[Property];
};
type X = {
    a: string;
    b: number;
};
type Y = J<X>;
```

In dit voorbeeld gebruikt het type `J<Type>` een mapped type met een template literal om de keys van `Type` te remap-pen. Het creëert nieuwe eigenschappen met een "prefix_" voor elke key, en hun bijbehorende waarden zijn functies die de oorspronkelijke eigenschapswaarden retourneren.

Het is vermeldenswaard dat TypeScript bij gebruik van een type-assertion geen controle uitvoert op extra eigenschappen (excess property checking). Daarom is het over het algemeen beter om een Typedeclaratie te gebruiken wanneer de structuur van het object vooraf bekend is.

#### Ambient declaraties

Ambient declaraties zijn bestanden die types beschrijven voor JavaScript-code; ze hebben het bestandsformaat `.d.ts`. Ze worden gewoonlijk geïmporteerd en gebruikt om bestaande JavaScript-bibliotheken te annoteren of om types toe te voegen aan bestaande JS-bestanden in je project.

Veel types voor veelvoorkomende bibliotheken zijn te vinden op:
[https://github.com/DefinitelyTyped/DefinitelyTyped/](https://github.com/DefinitelyTyped/DefinitelyTyped/)

en kunnen worden geïnstalleerd met:

```shell
npm install --save-dev @types/bibliotheeknaam
```

Voor je eigen gedefinieerde Ambient Declaraties kun je deze importeren met de "triple-slash" referentie:

<!-- skip -->
```typescript
/// <reference path="./library-types.d.ts" />
```

Je kunt Ambient Declaraties zelfs binnen JavaScript-bestanden gebruiken met `// @ts-check`.

Het trefwoord `declare` maakt typedefinities voor bestaande JavaScript-code mogelijk zonder deze te importeren, en dient als tijdelijke aanduiding voor types uit een ander bestand of globaal.

### Property Checking en Excess Property Checking

TypeScript is gebaseerd op een structureel typesysteem, maar "excess property checking" is een eigenschap van TypeScript waarmee het kan controleren of een object exact de eigenschappen heeft die in het type zijn gespecificeerd.

Excess Property Checking wordt uitgevoerd bij het toewijzen van object literals aan variabelen of bij het doorgeven ervan als argumenten aan functies.

<!-- skip -->
```typescript
type X = {
    a: string;
};
const y = { a: 'a', b: 'b' };
const x: X = y; // Geldig vanwege structurele typering
const w: X = { a: 'a', b: 'b' }; // Ongeldig vanwege excess property checking
```

### Zwakke Types (Weak Types)

Een type wordt als zwak beschouwd wanneer het uitsluitend een verzameling van optionele eigenschappen bevat:

```typescript
type X = {
    a?: string;
    b?: string;
};
```

TypeScript beschouwt het als een fout om iets toe te wijzen aan een zwak type wanneer er geen overlap is. Het volgende geeft bijvoorbeeld een foutmelding:

<!-- skip -->
```typescript
type Options = {
    a?: string;
    b?: string;
};

const fn = (options: Options) => undefined;

fn({ c: 'c' }); // Ongeldig
```

Hoewel het niet wordt aanbevolen, is het indien nodig mogelijk om deze controle te omzeilen met een type-assertion:

```typescript
type Options = {
    a?: string;
    b?: string;
};
const fn = (options: Options) => undefined;
fn({ c: 'c' } as Options); // Geldig
```

Of door `unknown` toe te voegen aan de index signature van het zwakke type:

```typescript
type Options = {
    [prop: string]: unknown;
    a?: string;
    b?: string;
};

const fn = (options: Options) => undefined;
fn({ c: 'c' }); // Geldig
```

### Strikte controle van Object Literals (Freshness)

Strikte controle van object literals, soms aangeduid als "freshness", is een functie in TypeScript die helpt bij het opsporen van extra of verkeerd gespelde eigenschappen die anders onopgemerkt zouden blijven bij normale structurele typecontroles.

Bij het maken van een object literal beschouwt de TypeScript-compiler deze als "vers" (fresh). Als de object literal wordt toegewezen aan een variabele of wordt doorgegeven als parameter, zal TypeScript een foutmelding geven als de object literal eigenschappen specificeert die niet bestaan in het doeltype.

"Freshness" verdwijnt echter wanneer een object literal wordt verbreed (widening) of wanneer een type-assertion wordt gebruikt.

Hier zijn enkele voorbeelden ter illustratie:

<!-- skip -->
```typescript
type X = { a: string };
type Y = { a: string; b: string };

let x: X;
x = { a: 'a', b: 'b' }; // Freshness-controle: Ongeldige toewijzing
var y: Y;
y = { a: 'a', bx: 'bx' }; // Freshness-controle: Ongeldige toewijzing

const fn = (x: X) => console.log(x.a);

fn(x);
fn(y); // Widening: Geen fouten, structureel compatibel

fn({ a: 'a', bx: 'b' }); // Freshness-controle: Ongeldig argument

let c: X = { a: 'a' };
let d: Y = { a: 'a', b: '' };
c = d; // Widening: Geen Freshness-controle
```

### Type Inference

TypeScript kan types afleiden (infereren) wanneer er geen annotatie is opgegeven tijdens:

* Variabele-initialisatie.
* Lid-initialisatie (member initialization).
* Het instellen van standaardwaarden voor parameters.
* Het return-type van een functie.

Bijvoorbeeld:

```typescript
let x = 'x'; // Het afgeleide type is string
```

De TypeScript-compiler analyseert de waarde of expressie en bepaalt het type op basis van de beschikbare informatie.

### Geavanceerdere Inferences

Wanneer meerdere expressies worden gebruikt bij type-inference, zoekt TypeScript naar de "best common types". Bijvoorbeeld:

```typescript
let x = [1, 'x', 1, null]; // Het afgeleide type is: (string | number | null)[]
```

Als de compiler geen "best common types" kan vinden, retourneert deze een union type. Bijvoorbeeld:

```typescript
let x = [new RegExp('x'), new Date()]; // Afgeleid type is: (RegExp | Date)[]
```

TypeScript maakt gebruik van "contextual typing" op basis van de locatie van de variabele om types af te leiden. In het volgende voorbeeld weet de compiler dat `e` van het type `MouseEvent` is vanwege het event-type `click` dat is gedefinieerd in het bestand `lib.d.ts`, dat ambient declaraties bevat voor verschillende veelvoorkomende JavaScript-constructies en de DOM:

```typescript
window.addEventListener('click', function (e) {}); // Het afgeleide type van e is MouseEvent
```

### Type-verbreding (Type Widening)

Type-verbreding (widening) is het proces waarbij TypeScript een type toekent aan een variabele die is geïnitialiseerd zonder dat er een type-annotatie is opgegeven. Het staat toe dat nauwe types worden omgezet naar bredere types, maar niet andersom.
In het volgende voorbeeld:

<!-- skip -->
```typescript
let x = 'x'; // TypeScript leidt dit af als string, een breed type
let y: 'y' | 'x' = 'y'; // y is een unie van literal types
y = x; // Ongeldig: Type 'string' is niet toewijsbaar aan type '"x" | "y"'.
```

TypeScript kent `string` toe aan `x` op basis van de enkele waarde die is opgegeven tijdens de initialisatie (`x`); dit is een voorbeeld van widening.

TypeScript biedt manieren om controle te hebben over het widening-proces, bijvoorbeeld door "const" te gebruiken.

### Const

Het gebruik van het trefwoord `const` bij het declareren van een variabele resulteert in een nauwere type-inference in TypeScript.

Bijvoorbeeld:

```typescript
const x = 'x'; // TypeScript leidt het type van x af als 'x', een nauwer type
let y: 'y' | 'x' = 'y';
y = x; // Geldig: Het type van x is afgeleid als 'x'
```

Door `const` te gebruiken om de variabele x te declareren, wordt het type vernauwd tot de specifieke literal waarde 'x'. Omdat het type van x is vernauwd, kan het zonder fouten worden toegewezen aan de variabele y.
De reden dat het type zo kan worden afgeleid, is dat `const` variabelen niet opnieuw kunnen worden toegewezen. Hierdoor kan hun type worden beperkt tot een specifiek literal type, in dit geval het literal type 'x'.

#### Const Modifier op Type Parameters

Vanaf versie 5.0 van TypeScript is het mogelijk om het `const` attribuut op een generieke type-parameter te specificeren. Dit maakt het mogelijk om het meest precieze type af te leiden. Laten we een voorbeeld bekijken zonder `const`:

```typescript
function identity<T>(value: T) {
    // Geen const hier
    return value;
}
const values = identity({ a: 'a', b: 'b' }); // Afgeleid type is: { a: string; b: string; }
```

Zoals je kunt zien, worden de eigenschappen `a` en `b` afgeleid met het type `string`.

Laten we nu het verschil zien met de `const` versie:

```typescript
function identity<const T>(value: T) {
    // Gebruik van const modifier op type parameters
    return value;
}
const values = identity({ a: 'a', b: 'b' }); // Afgeleid type is: { a: "a"; b: "b"; }
```

Nu zien we dat de eigenschappen `a` en `b` worden afgeleid als `const`, zodat `a` en `b` worden behandeld als string literals in plaats van alleen `string` types.

#### Const-assertion

Deze functie stelt je in staat om een variabele te declareren met een preciezer literal type op basis van de initialisatiewaarde. Hiermee geef je aan de compiler aan dat de waarde moet worden behandeld als een onveranderlijke (immutable) literal. Hier zijn enkele voorbeelden:

Op een enkele eigenschap:

```typescript
const v = {
    x: 3 as const,
};
v.x = 3;
```

Op een volledig object:

```typescript
const v = {
    x: 1,
    y: 2,
} as const;
```

Dit kan bijzonder nuttig zijn bij het definiëren van het type voor een tuple:

```typescript
const x = [1, 2, 3]; // number[]
const y = [1, 2, 3] as const; // Tuple van readonly [1, 2, 3]
```

### Expliciete Type-annotatie

We kunnen specifiek zijn en een type doorgeven. In het volgende voorbeeld is de eigenschap `x` van het type `number`:

```typescript
const v = {
    x: 1, // Afgeleid type: number (widening)
};
v.x = 3; // Geldig
```

We kunnen de type-annotatie specifieker maken door een unie van literal types te gebruiken:

<!-- skip -->
```typescript
const v: { x: 1 | 2 | 3 } = {
    x: 1, // x is nu een unie van literal types: 1 | 2 | 3
};
v.x = 3; // Geldig
v.x = 100; // Ongeldig
```

### Type-vernauwing (Type Narrowing)

Type-vernauwing (Type Narrowing) is het proces in TypeScript waarbij een algemeen type wordt verfijnd tot een specifieker type. Dit gebeurt wanneer TypeScript de code analyseert en vaststelt dat bepaalde voorwaarden of bewerkingen de type-informatie kunnen verfijnen.

Het vernauwen van types kan op verschillende manieren gebeuren, waaronder:

#### Voorwaarden

Door gebruik te maken van voorwaardelijke statements, zoals `if` of `switch`, kan TypeScript het type vernauwen op basis van de uitkomst van de voorwaarde. Bijvoorbeeld:

```typescript
let x: number | undefined = 10;

if (x !== undefined) {
    x += 100; // Het type is number, vernauwd door de voorwaarde
}
```

#### Throwing of returning

Het gooien (throwen) van een error of het vroegtijdig terugkeren (returnen) uit een vertakking kan TypeScript helpen een type te vernauwen. Bijvoorbeeld:

```typescript
let x: number | undefined = 10;

if (x === undefined) {
    throw 'error';
}
x += 100;
```

Andere manieren om types te vernauwen in TypeScript zijn:

* `instanceof` operator: Wordt gebruikt om te controleren of een object een instantie is van een specifieke class.
* `in` operator: Wordt gebruikt om te controleren of een eigenschap in een object bestaat.
* `typeof` operator: Wordt gebruikt om het type van een waarde tijdens runtime te controleren.
* Ingebouwde functies zoals `Array.isArray()`: Wordt gebruikt om te controleren of een waarde een array is.

#### Discriminated Union

Het gebruik van een "Discriminated Union" is een patroon in TypeScript waarbij een expliciete "tag" aan objecten wordt toegevoegd om onderscheid te maken tussen verschillende types binnen een unie. Dit patroon wordt ook wel een "tagged union" genoemd. In het volgende voorbeeld wordt de "tag" vertegenwoordigd door de eigenschap "type":

```typescript
type A = { type: 'type_a'; value: number };
type B = { type: 'type_b'; value: string };

const x = (input: A | B): string | number => {
    switch (input.type) {
        case 'type_a':
            return input.value + 100; // type is A
        case 'type_b':
            return input.value + 'extra'; // type is B
    }
};
```

#### User-Defined Type Guards

In gevallen waarin TypeScript niet in staat is om een type te bepalen, is het mogelijk om een hulpfunctie te schrijven die bekend staat als een "user-defined type guard". In het volgende voorbeeld zullen we een Type Predicate gebruiken om het type te vernauwen na het toepassen van een filtering:

```typescript
const data = ['a', null, 'c', 'd', null, 'f'];

const r1 = data.filter(x => x != null); // Het type is (string | null)[], TypeScript kon het type niet goed afleiden

const isValid = (item: string | null): item is string => item !== null; // Aangepaste type guard

const r2 = data.filter(isValid); // Het type is nu correct string[], door de predicate type guard te gebruiken konden we het type vernauwen
```

## Primitieve Types

TypeScript ondersteunt 7 primitieve types. Een primitief datatype verwijst naar een type dat geen object is en geen bijbehorende methoden heeft. In TypeScript zijn alle primitieve types onveranderlijk (immutable), wat betekent dat hun waarden niet kunnen worden gewijzigd zodra ze zijn toegewezen.

### string

Het primitieve type `string` slaat tekstuele gegevens op, en de waarde staat altijd tussen dubbele of enkele aanhalingstekens.

```typescript
const x: string = 'x';
const y: string = 'y';
```

Strings kunnen over meerdere regels worden verdeeld als ze worden omgeven door het backtick (`) karakter:

```typescript
let sentence: string = `xxx,
   yyy`;
```

### boolean

Het datatype `boolean` in TypeScript slaat een binaire waarde op: `true` of `false`.

```typescript
const isReady: boolean = true;
```

### number

Een datatype `number` in TypeScript wordt vertegenwoordigd door een 64-bits floating-point waarde. Een `number` type kan zowel gehele getallen als breuken vertegenwoordigen.
TypeScript ondersteunt ook hexadecimaal, binair en octaal, bijvoorbeeld:

```typescript
const decimal: number = 10;
const hexadecimal: number = 0xa00d; // Hexadecimaal begint met 0x
const binary: number = 0b1010; // Binair begint met 0b
const octal: number = 0o633; // Octaal begint met 0o
```

### bigInt

Een `bigInt` vertegenwoordigt numerieke waarden die erg groot zijn (2^53 – 1) en niet kunnen worden vertegenwoordigd met een `number`.

Een `bigInt` kan worden gemaakt door de ingebouwde functie `BigInt()` aan te roepen of door `n` toe te voegen aan het einde van een integer literal:

```typescript
const x: bigint = BigInt(9007199254740991);
const y: bigint = 9007199254740991n;
```

Opmerkingen:

* `bigInt` waarden kunnen niet worden gemengd met `number` en kunnen niet worden gebruikt met de ingebouwde `Math` functies; ze moeten naar hetzelfde type worden geconverteerd.
* `bigInt` waarden zijn alleen beschikbaar als de target-configuratie ES2020 of hoger is.

### Symbol

Symbols zijn unieke identificatoren die kunnen worden gebruikt als property-keys in objecten om naamconflicten te voorkomen.

```typescript
type Obj = {
    [sym: symbol]: number;
};

const a = Symbol('a');
const b = Symbol('b');
let obj: Obj = {};
obj[a] = 123;
obj[b] = 456;

console.log(obj[a]); // 123
console.log(obj[b]); // 456
```

### null en undefined

De types `null` en `undefined` vertegenwoordigen beide "geen waarde" of de afwezigheid van een waarde.

Het type `undefined` betekent dat de waarde niet is toegewezen of geïnitialiseerd, of geeft een onbedoelde afwezigheid van waarde aan.

Het type `null` betekent dat we weten dat het veld geen waarde heeft, dus de waarde is niet beschikbaar; het geeft een opzettelijke afwezigheid van waarde aan.

### Array

Een `array` is een datatype dat meerdere waarden van hetzelfde type (of verschillende types) kan opslaan. Het kan worden gedefinieerd met de volgende syntaxis:

```typescript
const x: string[] = ['a', 'b'];
const y: Array<string> = ['a', 'b'];
const j: Array<string | number> = ['a', 1, 'b', 2]; // Unie
```

TypeScript ondersteunt readonly-arrays met de volgende syntaxis:

<!-- skip -->
```typescript
const x: readonly string[] = ['a', 'b']; // Readonly modifier
const y: ReadonlyArray<string> = ['a', 'b'];
const j: ReadonlyArray<string | number> = ['a', 1, 'b', 2];
j.push('x'); // Ongeldig
```

TypeScript ondersteunt tuples en readonly-tuples:

```typescript
const x: [string, number] = ['a', 1];
const y: readonly [string, number] = ['a', 1];
```

### any

Het datatype `any` vertegenwoordigt letterlijk "elke" waarde. Het is de standaardwaarde wanneer TypeScript het type niet kan afleiden of wanneer het niet is gespecificeerd.

Bij het gebruik van `any` slaat de TypeScript-compiler de typecontrole over, dus er is geen typeveiligheid wanneer `any` wordt gebruikt. Gebruik `any` over het algemeen niet om de compiler de mond te snoeren wanneer er een fout optreedt; focus in plaats daarvan op het oplossen van de fout. Door `any` te gebruiken kun je contracten verbreken en verlies je de voordelen van TypeScript's autocomplete.

Het type `any` kan nuttig zijn tijdens een geleidelijke migratie van JavaScript naar TypeScript, omdat het de compiler stil kan houden.

Gebruik voor nieuwe projecten de TypeScript-configuratie `noImplicitAny`, die TypeScript in staat stelt foutmeldingen te geven op plekken waar `any` wordt gebruikt of afgeleid.

Het type `any` is vaak een bron van fouten die echte problemen met je types kunnen maskeren. Vermijd het gebruik ervan zoveel mogelijk.

## Type-annotaties

Bij variabelen die zijn gedeclareerd met `var`, `let` en `const`, is het mogelijk om optioneel een type toe te voegen:

```typescript
const x: number = 1;
```

TypeScript kan types erg goed afleiden, vooral bij eenvoudige declaraties, dus in de meeste gevallen zijn deze annotaties niet nodig.

Bij functies is het mogelijk om type-annotaties aan parameters toe te voegen:

```typescript
function sum(a: number, b: number) {
    return a + b;
}
```

Hieronder staat een voorbeeld met een anonieme functie (een zogenaamde lambda-functie):

```typescript
const sum = (a: number, b: number) => a + b;
```

Deze annotaties kunnen worden vermeden wanneer er een standaardwaarde voor een parameter aanwezig is:

```typescript
const sum = (a = 10, b: number) => a + b;
```

Return-type annotaties kunnen aan functies worden toegevoegd:

```typescript
const sum = (a = 10, b: number): number => a + b;
```

Dit is vooral nuttig voor complexere functies, omdat het expliciet opschrijven van het return-type vóór de implementatie kan helpen om beter over de functie na te denken.

Overweeg in het algemeen om type-signatures te annoteren, maar niet de lokale variabelen in de functie-body, en voeg altijd types toe aan object literals.

## Optionele Eigenschappen

Een object kan optionele eigenschappen specificeren door een vraagteken `?` toe te voegen aan het einde van de eigenschapsnaam:

```typescript
type X = {
    a: number;
    b?: number; // Optioneel
};
```

Het is mogelijk om een standaardwaarde op te geven wanneer een eigenschap optioneel is:

```typescript
type X = {
    a: number;
    b?: number;
};
const x = ({ a, b = 100 }: X) => a + b;
```

## Readonly Eigenschappen

Het is mogelijk om schrijven naar een eigenschap te voorkomen door de modifier `readonly` te gebruiken. Dit zorgt ervoor dat de eigenschap niet kan worden herschreven, maar biedt geen garantie voor totale onveranderlijkheid (immutability):

```typescript
interface Y {
    readonly a: number;
}

type X = {
    readonly a: number;
};

type J = Readonly<{
    a: number;
}>;

type K = {
    readonly [index: number]: string;
};
```

## Index Signatures

In TypeScript kunnen we als index signature `string`, `number` en `symbol` gebruiken:

```typescript
type K = {
    [name: string | number]: string;
};
const k: K = { x: 'x', 1: 'b' };
console.log(k['x']);
console.log(k[1]);
console.log(k['1']); // Zelfde resultaat als k[1]
```

Houd er rekening mee dat JavaScript een index met `number` automatisch converteert naar een index met `string`, dus `k[1]` of `k["1"]` retourneren dezelfde waarde.

## Types Uitbreiden

Het is mogelijk om een `interface` uit te breiden (leden kopiëren van een ander type):

```typescript
interface X {
    a: string;
}
interface Y extends X {
    b: string;
}
```

Het is ook mogelijk om uit te breiden van meerdere types:

```typescript
interface A {
    a: string;
}
interface B {
    b: string;
}
interface Y extends A, B {
    y: string;
}
```

Het trefwoord `extends` werkt alleen op interfaces en classes. Gebruik voor types een doorsnede (intersection):

```typescript
type A = {
    a: number;
};
type B = {
    b: number;
};
type C = A & B;
```

Het is mogelijk om een type uit te breiden met een interface, maar niet andersom:

```typescript
type A = {
    a: string;
};
interface B extends A {
    b: string;
}
```

## Literal Types

Een Literal Type is een verzameling van één element uit een collectief type. Het definieert een zeer exacte waarde die een JavaScript-primitief is.

Literal Types in TypeScript zijn getallen, strings en booleans.

Voorbeelden van literals:

```typescript
const a = 'a'; // String literal type
const b = 1; // Numeric literal type
const c = true; // Boolean literal type
```

String, Numeric en Boolean Literal Types worden gebruikt in unies, type-guards en type-aliases.
In het volgende voorbeeld zie je een type-alias unie; `O` kan alleen de opgegeven waarden hebben en geen andere string:

```typescript
type O = 'a' | 'b' | 'c';
```

## Literal Inference

Literal Inference is een functie in TypeScript waarmee het type van een variabele of parameter kan worden afgeleid op basis van zijn waarde.

In het volgende voorbeeld zien we dat TypeScript `x` als een literal type beschouwt omdat de waarde later niet meer kan worden gewijzigd, terwijl `y` wordt afgeleid als `string` omdat deze op elk moment kan worden gewijzigd.

```typescript
const x = 'x'; // Literal type 'x', omdat deze waarde niet kan worden gewijzigd
let y = 'y'; // Type string, omdat we deze waarde kunnen wijzigen
```

In het volgende voorbeeld zien we dat `o.x` is afgeleid als een `string` (en niet als een literal 'a'), omdat TypeScript ervan uitgaat dat de waarde op elk moment later kan worden gewijzigd.

<!-- skip -->
```typescript
type X = 'a' | 'b';

let o = {
    x: 'a', // Dit is een bredere string
};

const fn = (x: X) => `${x}-foo`;

console.log(fn(o.x)); // Argument of type 'string' is not assignable to parameter of type 'X'
```

Zoals je ziet, geeft de code een foutmelding bij het doorgeven van `o.x` aan `fn` omdat X een nauwer type is.

We kunnen dit probleem oplossen door een type-assertion te gebruiken met `const` of het type `X`:

<!-- skip -->
```typescript
let o = {
    x: 'a' as const,
};
```

of:

<!-- skip -->
```typescript
let o = {
    x: 'a' as X,
};
```

## strictNullChecks

`strictNullChecks` is een TypeScript-compileroptie die strikte null-controle afdwingt. Wanneer deze optie is ingeschakeld, kunnen variabelen en parameters alleen `null` of `undefined` toegewezen krijgen als ze expliciet zijn gedeclareerd als zijnde van dat type met behulp van de unie-type `null | undefined`. Als een variabele of parameter niet expliciet als nullable is gedeclareerd, zal TypeScript een foutmelding genereren om potentiële runtime-fouten te voorkomen.

## Enums

In TypeScript is een `enum` een verzameling benoemde constante waarden.

```typescript
enum Color {
    Red = '#ff0000',
    Green = '#00ff00',
    Blue = '#0000ff',
}
```

Enums kunnen op verschillende manieren worden gedefinieerd:

### Numerieke enums

In TypeScript is een numerieke enum een enum waarbij aan elke constante een numerieke waarde wordt toegekend, standaard beginnend bij 0.

```typescript
enum Size {
    Small, // waarde begint bij 0
    Medium,
    Large,
}
```

Het is mogelijk om aangepaste waarden op te geven door deze expliciet toe te wijzen:

```typescript
enum Size {
    Small = 10,
    Medium,
    Large,
}
console.log(Size.Medium); // 11
```

### String enums

In TypeScript is een string enum een enum waarbij aan elke constante een string-waarde wordt toegekend.

```typescript
enum Language {
    English = 'EN',
    Spanish = 'ES',
}
```

Opmerking: TypeScript staat het gebruik van heterogene enums toe, waarbij string- en numerieke leden naast elkaar kunnen bestaan.

### Constante enums

Een constante enum in TypeScript is een speciaal type enum waarvan alle waarden bekend zijn tijdens compilatie en inline worden geplaatst waar de enum wordt gebruikt, wat resulteert in efficiëntere code.

```typescript
const enum Language {
    English = 'EN',
    Spanish = 'ES',
}
console.log(Language.English);
```

Zal worden gecompileerd naar:

```typescript
console.log('EN' /* Language.English */);
```

Opmerkingen:
Constante enums hebben hard-coded waarden, waardoor de enum zelf wordt verwijderd. Dit kan efficiënter zijn in zelfstandige bibliotheken, maar is over het algemeen niet wenselijk. Ook kunnen constante enums geen berekende leden hebben.

### Reverse mapping

In TypeScript verwijst "reverse mapping" in enums naar de mogelijkheid om de naam van een enum-lid op te halen aan de hand van zijn waarde. Standaard hebben enum-leden forward mappings van naam naar waarde, maar reverse mappings kunnen worden gemaakt door expliciet waarden in te stellen voor elk lid. Reverse mappings zijn nuttig wanneer je een enum-lid moet opzoeken via zijn waarde, of wanneer je over alle enum-leden wilt itereren. Merk op dat alleen numerieke enum-leden reverse mappings genereren, terwijl string enum-leden helemaal geen reverse mapping genereren.

De volgende enum:

```typescript
enum Grade {
    A = 90,
    B = 80,
    C = 70,
    F = 'fail',
}
```

Compileert naar:

<!-- skip -->
```javascript
'use strict';
var Grade;
(function (Grade) {
    Grade[(Grade['A'] = 90)] = 'A';
    Grade[(Grade['B'] = 80)] = 'B';
    Grade[(Grade['C'] = 70)] = 'C';
    Grade['F'] = 'fail';
})(Grade || (Grade = {}));
```

Daarom werkt het mappen van waarden naar keys voor numerieke enum-leden, maar niet voor string enum-leden:

<!-- skip -->
```typescript
enum Grade {
    A = 90,
    B = 80,
    C = 70,
    F = 'fail',
}
const myGrade = Grade.A;
console.log(Grade[myGrade]); // A
console.log(Grade[90]); // A

const failGrade = Grade.F;
console.log(failGrade); // fail
console.log(Grade[failGrade]); // Element heeft impliciet een 'any' type omdat de index-expressie niet van het type 'number' is.
```

### Ambient enums

Een ambient enum in TypeScript is een type enum dat is gedefinieerd in een declaratiebestand (*.d.ts) zonder bijbehorende implementatie. Het stelt je in staat om een verzameling benoemde constanten te definiëren die op een typeveilige manier in verschillende bestanden kunnen worden gebruikt, zonder dat je de implementatiedetails in elk bestand hoeft te importeren.

### Berekende en constante leden

In TypeScript is een berekend lid een lid van een enum met een waarde die tijdens runtime wordt berekend, terwijl een constant lid een lid is waarvan de waarde tijdens compilatie wordt ingesteld en niet kan worden gewijzigd tijdens runtime. Berekende leden zijn toegestaan in gewone enums, terwijl constante leden zijn toegestaan in zowel gewone als constante enums.

```typescript
// Constante leden
enum Color {
    Red = 1,
    Green = 5,
    Blue = Red + Green,
}
console.log(Color.Blue); // 6 (gegenereerd tijdens compilatie)
```

```typescript
// Berekende leden
enum Color {
    Red = 1,
    Green = Math.pow(2, 2),
    Blue = Math.floor(Math.random() * 3) + 1,
}
console.log(Color.Blue); // willekeurig getal gegenereerd tijdens runtime
```

Enums worden gekenmerkt door unies die bestaan uit hun ledentypes. De waarden van elk lid kunnen worden bepaald via constante of niet-constante expressies, waarbij aan leden met constante waarden literal types worden toegekend. Ter illustratie: overweeg de declaratie van type E en zijn subtypes E.A, E.B en E.C. In dit geval vertegenwoordigt E de unie E.A | E.B | E.C.

```typescript
const identity = (value: number) => value;

enum E {
    A = 2 * 5, // Numeric literal
    B = 'bar', // String literal
    C = identity(42), // Opaque computed
}

console.log(E.C); // 42
```

## Narrowing

TypeScript narrowing is het proces van het verfijnen van het type van een variabele binnen een voorwaardelijk blok. Dit is nuttig bij het werken met union types, waarbij een variabele meer dan één type kan hebben.

TypeScript herkent verschillende manieren om het type te vernauwen:

### typeof type guards

De `typeof` type guard is een specifieke type guard in TypeScript die het type van een variabele controleert op basis van zijn ingebouwde JavaScript-type.

```typescript
const fn = (x: number | string) => {
    if (typeof x === 'number') {
        return x + 1; // x is number
    }
    return -1;
};
```

### Truthiness narrowing

Truthiness narrowing in TypeScript werkt door te controleren of een variabele "truthy" of "falsy" is om het type dienovereenkomstig te vernauwen.

```typescript
const toUpperCase = (name: string | null) => {
    if (name) {
        return name.toUpperCase();
    } else {
        return null;
    }
};
```

### Equality narrowing

Equality narrowing in TypeScript werkt door te controleren of een variabele gelijk is aan een specifieke waarde of niet, om het type dienovereenkomstig te vernauwen.

Het wordt gebruikt in combinatie met `switch` statements en gelijkheidsoperators zoals `===`, `!==`, `==`, en `!=` om types te vernauwen.

```typescript
const checkStatus = (status: 'success' | 'error') => {
    switch (status) {
        case 'success':
            return true;
        case 'error':
            return null;
    }
};
```

### In-operator narrowing

De `in`-operator narrowing in TypeScript is een manier om het type van een variabele te vernauwen op basis van de vraag of een eigenschap bestaat binnen het type van de variabele.

```typescript
type Dog = {
    name: string;
    breed: string;
};

type Cat = {
    name: string;
    likesCream: boolean;
};

const getAnimalType = (pet: Dog | Cat) => {
    if ('breed' in pet) {
        return 'dog';
    } else {
        return 'cat';
    }
};
```

### instanceof narrowing

De `instanceof`-operator narrowing in TypeScript is een manier om het type van een variabele te vernauwen op basis van zijn constructorfunctie, door te controleren of een object een instantie is van een bepaalde class of interface.

```typescript
class Square {
    constructor(public width: number) {}
}
class Rectangle {
    constructor(
        public width: number,
        public height: number
    ) {}
}
function area(shape: Square | Rectangle) {
    if (shape instanceof Square) {
        return shape.width * shape.width;
    } else {
        return shape.width * shape.height;
    }
}
const square = new Square(5);
const rectangle = new Rectangle(5, 10);
console.log(area(square)); // 25
console.log(area(rectangle)); // 50
```

## Toewijzingen (Assignments)

TypeScript narrowing met behulp van toewijzingen is een manier om het type van een variabele te vernauwen op basis van de waarde die eraan is toegewezen. Wanneer een variabele een waarde krijgt toegewezen, leidt TypeScript het type af op basis van de toegewezen waarde, en vernauwt het het type van de variabele om overeen te komen met het afgeleide type.

```typescript
let value: string | number;
value = 'hello';
if (typeof value === 'string') {
    console.log(value.toUpperCase());
}
value = 42;
if (typeof value === 'number') {
    console.log(value.toFixed(2));
}
```

## Control Flow Analysis

Control Flow Analysis in TypeScript is een manier om de code-flow statisch te analyseren om de types van variabelen af te leiden, waardoor de compiler de types van die variabelen naar behoefte kan vernauwen op basis van de resultaten van de analyse.

Vóór TypeScript 4.4 werd code-flow analyse alleen toegepast op code binnen een if-statement, maar vanaf TypeScript 4.4 kan het ook worden toegepast op voorwaardelijke expressies en indirecte verwijzingen naar discriminerende eigenschappen via const-variabelen.

Bijvoorbeeld:

```typescript
const f1 = (x: unknown) => {
    const isString = typeof x === 'string';
    if (isString) {
        x.length;
    }
};

const f2 = (
    obj: { kind: 'foo'; foo: string } | { kind: 'bar'; bar: number }
) => {
    const isFoo = obj.kind === 'foo';
    if (isFoo) {
        obj.foo;
    } else {
        obj.bar;
    }
};
```

Enkele voorbeelden waar narrowing niet optreedt:

<!-- skip -->
```typescript
const f1 = (x: unknown) => {
    let isString = typeof x === 'string';
    if (isString) {
        x.length; // Fout, geen narrowing omdat isString geen const is
    }
};

const f6 = (
    obj: { kind: 'foo'; foo: string } | { kind: 'bar'; bar: number }
) => {
    const isFoo = obj.kind === 'foo';
    obj = obj;
    if (isFoo) {
        obj.foo; // Fout, geen narrowing omdat obj opnieuw is toegewezen in de functie-body
    }
};
```

Opmerkingen: Tot vijf niveaus van indirectie worden geanalyseerd in voorwaardelijke expressies.

## Type Predicates

Type Predicates in TypeScript zijn functies die een boolean waarde retourneren en worden gebruikt om het type van een variabele te vernauwen naar een specifieker type.

```typescript
const isString = (value: unknown): value is string => typeof value === 'string';

const foo = (bar: unknown) => {
    if (isString(bar)) {
        console.log(bar.toUpperCase());
    } else {
        console.log('not a string');
    }
};
```

## Gediscrimineerde Unies (Discriminated Unions)

Gediscrimineerde Unies (Discriminated Unions) in TypeScript zijn een type union type dat een gemeenschappelijke eigenschap gebruikt, bekend als de discriminant, om de verzameling mogelijke types voor de unie te vernauwen.

```typescript
type Square = {
    kind: 'square'; // Discriminant
    size: number;
};

type Circle = {
    kind: 'circle'; // Discriminant
    radius: number;
};

type Shape = Square | Circle;

const area = (shape: Shape) => {
    switch (shape.kind) {
        case 'square':
            return Math.pow(shape.size, 2);
        case 'circle':
            return Math.PI * Math.pow(shape.radius, 2);
    }
};

const square: Square = { kind: 'square', size: 5 };
const circle: Circle = { kind: 'circle', radius: 2 };

console.log(area(square)); // 25
console.log(area(circle)); // 12.566370614359172
```

## Het never Type

Wanneer een variabele wordt vernauwd naar een type dat geen enkele waarde kan bevatten, zal de TypeScript-compiler afleiden dat de variabele van het type `never` moet zijn. Dit komt omdat het `never` type een waarde vertegenwoordigt die nooit kan worden geproduceerd.

```typescript
const printValue = (val: string | number) => {
    if (typeof val === 'string') {
        console.log(val.toUpperCase());
    } else if (typeof val === 'number') {
        console.log(val.toFixed(2));
    } else {
        // val heeft hier het type never omdat het nooit iets anders kan zijn dan een string of een getal
        const neverVal: never = val;
        console.log(`Onverwachte waarde: ${neverVal}`);
    }
};
```

## Exhaustiveness checking

Exhaustiveness checking is een functie in TypeScript die ervoor zorgt dat alle mogelijke gevallen van een gediscrimineerde unie worden afgehandeld in een `switch` statement of een `if` statement.

```typescript
type Direction = 'up' | 'down';

const move = (direction: Direction) => {
    switch (direction) {
        case 'up':
            console.log('Moving up');
            break;
        case 'down':
            console.log('Moving down');
            break;
        default:
            const exhaustiveCheck: never = direction;
            console.log(exhaustiveCheck); // Deze regel zal nooit worden uitgevoerd
    }
};
```

Het `never` type wordt gebruikt om te garanderen dat de default-case uitputtend (exhaustive) is en dat TypeScript een foutmelding geeft als er een nieuwe waarde wordt toegevoegd aan het Direction-type zonder dat deze in het switch-statement wordt afgehandeld.

## Object Types

In TypeScript beschrijven object types de vorm van een object. Ze specificeren de namen en types van de eigenschappen van het object, evenals of die eigenschappen verplicht of optioneel zijn.

In TypeScript kun je object types op twee manieren definiëren:

Interface, die de vorm van een object definieert door de namen, types en optionele status van zijn eigenschappen te specificeren.

```typescript
interface User {
    name: string;
    age: number;
    email?: string;
}
```

Type-alias, vergelijkbaar met een interface, definieert de vorm van een object. Het kan echter ook een nieuw aangepast type maken dat is gebaseerd op een bestaand type of een combinatie van bestaande types. Dit omvat het definiëren van union types, intersection types en andere complexe types.

```typescript
type Point = {
    x: number;
    y: number;
};
```

Het is ook mogelijk om een type anoniem te definiëren:

```typescript
const sum = (x: { a: number; b: number }) => x.a + x.b;
console.log(sum({ a: 5, b: 1 }));
```

## Tuple Type (Anoniem)

Een Tuple Type is een type dat een array vertegenwoordigt met een vast aantal elementen en hun bijbehorende types. Een tuple type dwingt een specifiek aantal elementen en hun respectievelijke types in een vaste volgorde af. Tuple types zijn nuttig wanneer je een verzameling waarden met specifieke types wilt vertegenwoordigen, waarbij de positie van elk element in de array een specifieke betekenis heeft.

```typescript
type Point = [number, number];
```

## Named Tuple Type (Gelabeld)

Tuple types kunnen optionele labels of namen bevatten voor elk element. Deze labels zijn bedoeld voor de leesbaarheid en ondersteuning door tools, en hebben geen invloed op de bewerkingen die je ermee kunt uitvoeren.

```typescript
type T = string;
type Tuple1 = [T, T];
type Tuple2 = [a: T, b: T];
type Tuple3 = [a: T, T]; // Named Tuple plus Anonieme Tuple
```

## Vaste lengte Tuple

Een Vaste lengte Tuple is een specifiek type tuple dat een vast aantal elementen van specifieke types afdwingt en geen wijzigingen toestaat aan de lengte van de tuple zodra deze is gedefinieerd.

Vaste lengte Tuples zijn nuttig wanneer je een verzameling waarden moet vertegenwoordigen met een specifiek aantal elementen en specifieke types, en je wilt garanderen dat de lengte en types van de tuple niet onbedoeld kunnen worden gewijzigd.

<!-- skip -->
```typescript
const x = [10, 'hello'] as const;
x.push(2); // Fout
```

## Union Type

Een Union Type is een type dat een waarde vertegenwoordigt die een van meerdere types kan zijn. Union types worden aangeduid met het `|` symbool tussen elk mogelijk type.

```typescript
let x: string | number;
x = 'hello'; // Geldig
x = 123; // Geldig
```

## Intersection Types

Een Intersection Type is een type dat een waarde vertegenwoordigt die alle eigenschappen van twee of meer types heeft. Intersection types worden aangeduid met het `&` symbool tussen elk type.

```typescript
type X = {
    a: string;
};

type Y = {
    b: string;
};

type J = X & Y; // Doorsnede (Intersection)

const j: J = {
    a: 'a',
    b: 'b',
};
```

## Type Indexing

Type indexing verwijst naar de mogelijkheid om types te definiëren die kunnen worden geïndexeerd met een key die niet vooraf bekend is, waarbij een index-signature wordt gebruikt om het type te specificeren voor eigenschappen die niet expliciet zijn gedeclareerd.

```typescript
type Dictionary<T> = {
    [key: string]: T;
};
const myDict: Dictionary<string> = { a: 'a', b: 'b' };
console.log(myDict['a']); // Retourneert a
```

## Type van Waarde

Type van waarde in TypeScript verwijst naar de automatische afleiding van een type uit een waarde of expressie door middel van type inference.

```typescript
const x = 'x'; // TypeScript leidt 'x' af als een string-literal met 'const' (onveranderlijk), maar verbreedt het tot 'string' met 'let' (opnieuw toewijsbaar).
```

## Type van Functie Return

Type van functie return verwijst naar de mogelijkheid om automatisch het return-type van een functie af te leiden op basis van de implementatie. Hierdoor kan TypeScript het type bepalen van de waarde die door de functie wordt geretourneerd zonder expliciete type-annotaties.

```typescript
const add = (x: number, y: number) => x + y; // TypeScript kan afleiden dat het return-type van de functie een getal is
```

## Type van Module

Type van module verwijst naar de mogelijkheid om de geëxporteerde waarden van een module te gebruiken om automatisch hun types af te leiden. Wanneer een module een waarde met een specifiek type exporteert, kan TypeScript die informatie gebruiken om automatisch het type van die waarde af te leiden wanneer deze in een andere module wordt geïmporteerd.

<!-- skip -->
```typescript
// calc.ts
export const add = (x: number, y: number) => x + y;
// index.ts
import { add } from 'calc';
const r = add(1, 2); // r is een number
```

## Mapped Types

Mapped Types in TypeScript stellen je in staat om nieuwe types te maken op basis van een bestaand type door elke eigenschap te transformeren met behulp van een mapping-functie. Door bestaande types te mappen, kun je nieuwe types creëren die dezelfde informatie in een ander formaat vertegenwoordigen. Om een mapped type te maken, benader je de eigenschappen van een bestaand type met de `keyof` operator en wijzig je deze vervolgens om een nieuw type te produceren.
In het volgende voorbeeld:

```typescript
type MyMappedType<T> = {
    [P in keyof T]: T[P][];
};
type MyType = {
    foo: string;
    bar: number;
};
type MyNewType = MyMappedType<MyType>;
const x: MyNewType = {
    foo: ['hello', 'world'],
    bar: [1, 2, 3],
};
```

definiëren we `MyMappedType` om over de eigenschappen van `T` te mappen, waarbij een nieuw type wordt gemaakt waarbij elke eigenschap een array is van het oorspronkelijke type. Hiermee maken we `MyNewType` om dezelfde informatie te vertegenwoordigen als `MyType`, maar met elke eigenschap als een array.

## Mapped Type Modifiers

Mapped Type Modifiers in TypeScript maken de transformatie van eigenschappen binnen een bestaand type mogelijk:

* `readonly` of `+readonly`: Dit maakt een eigenschap in het gemapte type alleen-lezen.
* `-readonly`: Dit zorgt ervoor dat een eigenschap in het gemapte type mutabel (wijzigbaar) is.
* `?`: Dit markeert een eigenschap in het gemapte type als optioneel.

Voorbeelden:

```typescript
type ReadOnly<T> = { readonly [P in keyof T]: T[P] }; // Alle eigenschappen gemarkeerd als alleen-lezen

type Mutable<T> = { -readonly [P in keyof T]: T[P] }; // Alle eigenschappen gemarkeerd als mutabel

type MyPartial<T> = { [P in keyof T]?: T[P] }; // Alle eigenschappen gemarkeerd als optioneel
```

## Conditional Types

Conditional Types zijn een manier om een type te maken dat afhankelijk is van een voorwaarde, waarbij het te maken type wordt bepaald op basis van het resultaat van de voorwaarde. Ze worden gedefinieerd met het trefwoord `extends` en een ternaire operator om conditioneel tussen twee types te kiezen.

```typescript
type IsArray<T> = T extends any[] ? true : false;

const myArray = [1, 2, 3];
const myNumber = 42;

type IsMyArrayAnArray = IsArray<typeof myArray>; // Type true
type IsMyNumberAnArray = IsArray<typeof myNumber>; // Type false
```

## Distributieve Conditional Types

Distributieve Conditional Types zijn een functie die het mogelijk maakt om een type te distribueren over een unie van types, door een transformatie toe te passen op elk lid van de unie afzonderlijk.
Dit kan vooral nuttig zijn bij het werken met mapped types of hogere-orde types.

```typescript
type Nullable<T> = T extends any ? T | null : never;
type NumberOrBool = number | boolean;
type NullableNumberOrBool = Nullable<NumberOrBool>; // number | boolean | null
```

## infer Type-inference in Conditional Types

Het trefwoord `infer` wordt gebruikt in conditional types om het type van een generieke parameter af te leiden (te extraheren) uit een type dat ervan afhankelijk is. Hierdoor kun je flexibelere en herbruikbare typedefinities schrijven.

```typescript
type ElementType<T> = T extends (infer U)[] ? U : never;
type Numbers = ElementType<number[]>; // number
type Strings = ElementType<string[]>; // string
```

## Vooraf gedefinieerde Conditional Types

In TypeScript zijn vooraf gedefinieerde conditional types ingebouwde conditional types die door de taal worden geleverd. Ze zijn ontworpen om veelvoorkomende type-transformaties uit te voeren op basis van de kenmerken van een gegeven type.

`Exclude<UnionType, ExcludedType>`: Dit type verwijdert alle types uit Type die toewijsbaar zijn aan ExcludedType.

`Extract<Type, Union>`: Dit type extraheert alle types uit Union die toewijsbaar zijn aan Type.

`NonNullable<Type>`: Dit type verwijdert null en undefined uit Type.

`ReturnType<Type>`: Dit type extraheert het return-type van een functie Type.

`Parameters<Type>`: Dit type extraheert de parametertypes van een functie Type.

`Required<Type>`: Dit type maakt alle eigenschappen in Type verplicht.

`Partial<Type>`: Dit type maakt alle eigenschappen in Type optioneel.

`Readonly<Type>`: Dit type maakt alle eigenschappen in Type readonly.

## Template Union Types

Template union types kunnen worden gebruikt om tekst binnen het typesysteem samen te voegen en te manipuleren, bijvoorbeeld:

```typescript
type Status = 'active' | 'inactive';
type Products = 'p1' | 'p2';
type ProductId = `id-${Products}-${Status}`; // "id-p1-active" | "id-p1-inactive" | "id-p2-active" | "id-p2-inactive"
```

## Any type

Het type `any` is een speciaal type (universeel supertype) dat kan worden gebruikt om elk type waarde te vertegenwoordigen (primitieven, objecten, arrays, functies, errors, symbols). Het wordt vaak gebruikt in situaties waarin het type van een waarde niet bekend is tijdens compilatie, of bij het werken met waarden uit externe API's of bibliotheken die geen TypeScript-typings hebben.

Door het type `any` te gebruiken, geef je aan de TypeScript-compiler aan dat waarden zonder enige beperking moeten worden weergegeven. Overweeg het volgende om de typeveiligheid in je code te maximaliseren:

* Beperk het gebruik van `any` tot specifieke gevallen waarin het type werkelijk onbekend is.
* Retourneer geen `any` types uit een functie, omdat je de typeveiligheid verliest in de code die die functie gebruikt, wat je totale typeveiligheid verzwakt.
* Gebruik in plaats van `any` de directive `@ts-ignore` als je de compiler stil moet houden.

```typescript
let value: any;
value = true; // Geldig
value = 7; // Geldig
```

## Unknown type

In TypeScript vertegenwoordigt het type `unknown` een waarde waarvan het type onbekend is. In tegenstelling tot het type `any`, dat elk type waarde toestaat, vereist `unknown` een type-check of assertion voordat het op een specifieke manier kan worden gebruikt. Er zijn dus geen bewerkingen toegestaan op een `unknown` zonder eerst een bewering (assertion) te doen of te vernauwen naar een specifieker type.

Het type `unknown` is alleen toewijsbaar aan any en aan zichzelf; het is een typeveilig alternatief voor `any`.

<!-- skip -->
```typescript
let value: unknown;

let value1: unknown = value; // Geldig
let value2: any = value; // Geldig
let value3: boolean = value; // Ongeldig
let value4: number = value; // Ongeldig
```

```typescript
const add = (a: unknown, b: unknown): number | undefined =>
    typeof a === 'number' && typeof b === 'number' ? a + b : undefined;
console.log(add(1, 2)); // 3
console.log(add('x', 2)); // undefined
```

## Void type

Het type `void` wordt gebruikt om aan te geven dat een functie geen waarde retourneert.

```typescript
const sayHello = (): void => {
    console.log('Hello!');
};
```

## Never type

Het type `never` vertegenwoordigt waarden die nooit voorkomen. Het wordt gebruikt om functies of expressies aan te duiden die nooit iets teruggeven of een error gooien.

Bijvoorbeeld een oneindige loop:

```typescript
const infiniteLoop = (): never => {
    while (true) {
        // doe iets
    }
};
```

Het gooien van een error:

```typescript
const throwError = (message: string): never => {
    throw new Error(message);
};
```

Het `never` type is nuttig bij het waarborgen van typeveiligheid en het opvangen van potentiële fouten in je code. Het helpt TypeScript om preciezere types te analyseren en af te leiden wanneer het wordt gebruikt in combinatie met andere types en control-flow statements, bijvoorbeeld:

```typescript
type Direction = 'up' | 'down';
const move = (direction: Direction): void => {
    switch (direction) {
        case 'up':
            // beweeg omhoog
            break;
        case 'down':
            // beweeg omlaag
            break;
        default:
            const exhaustiveCheck: never = direction;
            throw new Error(`Niet-afgehandelde richting: ${exhaustiveCheck}`);
    }
};
```

