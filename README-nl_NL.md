# Het Beknopte TypeScript Boek

Het Beknopte TypeScript Boek biedt een uitgebreid en bondig overzicht van de mogelijkheden van TypeScript. Het biedt heldere uitleg over alle aspecten van de nieuwste versie van de taal, van het krachtige typesysteem tot geavanceerde functies. Of je nu een beginner bent of een ervaren ontwikkelaar, dit boek is een onschatbare bron om je begrip van en vaardigheid in TypeScript te vergroten.

Dit boek is volledig gratis en Open Source.

Ik geloof dat kwalitatief hoogstaand technisch onderwijs voor iedereen toegankelijk moet zijn, en daarom houd ik dit boek gratis en open.

Als het boek je heeft geholpen een bug op te lossen, een lastig concept te begrijpen of verder te komen in je carrière, overweeg dan om mijn werk te steunen door te betalen wat je wilt (gesuggereerde prijs: 15 USD) of door een kopje koffie te sponsoren. Jouw steun helpt me om de inhoud up-to-date te houden en uit te breiden met nieuwe voorbeelden en diepere uitleg.

[![Buy Me a Coffee](https://img.shields.io/badge/buy_me_a_coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/simonepoggiali)

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=QW82ZS956XLFY&no_recurring=0&currency_code=EUR)

## Vertalingen

Dit boek is vertaald in verschillende taalversies, waaronder:

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
    - [Advies voor Migratie naar TypeScript](#advies-voor-migratie-naar-typescript)
  - [Het Typesysteem Verkennen](#het-typesysteem-verkennen)
    - [De TypeScript Language Service](#de-typescript-language-service)
    - [Structurele Typering](#structurele-typering)
    - [Fundamentele Vergelijkingsregels van TypeScript](#fundamentele-vergelijkingsregels-van-typescript)
    - [Types als Verzamelingen](#types-als-verzamelingen)
    - [Een Type Toewijzen: Typedeclaraties en Type-assertions](#een-type-toewijzen-typedeclaraties-en-type-assertions)
      - [Typedeclaratie](#typedeclaratie)
      - [Type-assertion](#type-assertion)
      - [Ambient Declarations](#ambient-declarations)
    - [Property Checking en Excess Property Checking](#property-checking-en-excess-property-checking)
    - [Weak Types](#weak-types)
    - [Strict Object Literal Checking (Freshness)](#strict-object-literal-checking-freshness)
    - [Type Inference](#type-inference)
    - [Geavanceerdere Inferences](#geavanceerdere-inferences)
    - [Type Widening](#type-widening)
    - [Const](#const)
      - [Const Modifier op Type Parameters](#const-modifier-on-type-parameters)
      - [Const Assertion](#const-assertion)
    - [Expliciete Type-annotatie](#explicit-type-annotation)
    - [Type Narrowing](#type-narrowing)
      - [Voorwaarden](#conditions)
      - [Throwing of Returning](#throwing-of-returning)
      - [Discriminated Union](#discriminated-union)
      - [User-Defined Type Guards](#user-defined-type-guards)
  - [Primitieve Types](#primitieve-types)
    - [string](#string)
    - [boolean](#boolean)
    - [number](#number)
    - [bigInt](#bigint)
    - [Symbol](#symbol)
    - [null en undefined](#null-and-undefined)
    - [Array](#array)
    - [any](#any)
  - [Type-annotaties](#type-annotations)
  - [Optionele Eigenschappen](#optional-properties)
  - [Readonly Eigenschappen](#readonly-properties)
  - [Index Signatures](#index-signatures)
  - [Types Uitbreiden](#extending-types)
  - [Literal Types](#literal-types)
  - [Literal Inference](#literal-inference)
  - [strictNullChecks](#strictnullchecks)
  - [Enums](#enums)
    - [Numerieke Enums](#numeric-enums)
    - [String Enums](#string-enums)
    - [Constante Enums](#constant-enums)
    - [Reverse Mapping](#reverse-mapping)
    - [Ambient Enums](#ambient-enums)
    - [Berekende en Constante Leden](#computed-and-constant-members)
  - [Narrowing](#narrowing)
    - [typeof Type Guards](#typeof-type-guards)
    - [Truthiness Narrowing](#truthiness-narrowing)
    - [Equality Narrowing](#equality-narrowing)
    - [In Operator Narrowing](#in-operator-narrowing)
    - [instanceof Narrowing](#instanceof-narrowing)
  - [Assignments](#assignments)
  - [Control Flow Analysis](#control-flow-analysis)
  - [Type Predicates](#type-predicates)
  - [Discriminated Unions](#discriminated-unions)
  - [Het never Type](#the-never-type)
  - [Exhaustiveness Checking](#exhaustiveness-checking)
  - [Object Types](#object-types)
  - [Tuple Type (Anoniem)](#tuple-type-anonymous)
  - [Named Tuple Type (Gelabeld)](#named-tuple-type-labeled)
  - [Vaste Lengte Tuple](#fixed-length-tuple)
  - [Union Type](#union-type)
  - [Intersection Types](#intersection-types)
  - [Type Indexing](#type-indexing)
  - [Type van Waarde](#type-from-value)
  - [Type van Functie Return](#type-from-func-return)
  - [Type van Module](#type-from-module)
  - [Mapped Types](#mapped-types)
  - [Mapped Type Modifiers](#mapped-type-modifiers)
  - [Conditional Types](#conditional-types)
  - [Distributieve Conditional Types](#distributive-conditional-types)
  - [infer Type Inference in Conditional Types](#infer-type-inference-in-conditional-types)
  - [Vooraf Gedefinieerde Conditional Types](#predefined-conditional-types)
  - [Template Union Types](#template-union-types)
  - [Any type](#any-type)
  - [Unknown type](#unknown-type)
  - [Void type](#void-type)
  - [Never type](#never-type)
  - [Interface en Type](#interface-and-type)
    - [Gemeenschappelijke Syntaxis](#common-syntax)
    - [Basis Types](#basic-types)
    - [Objecten en Interfaces](#objects-and-interfaces)
    - [Union en Intersection Types](#union-and-intersection-types)
  - [Ingebouwde Type Primitieven](#built-in-type-primitives)
  - [Veelvoorkomende Ingebouwde JS Objecten](#common-built-in-js-objects)
  - [Overloads](#overloads)
  - [Samenvoegen en Uitbreiden](#merging-and-extension)
  - [Verschillen tussen Type en Interface](#differences-between-type-and-interface)
  - [Class](#class)
    - [Algemene Class Syntaxis](#class-common-syntax)
    - [Constructor](#constructor)
    - [Private en Protected Constructoren](#private-and-protected-constructors)
    - [Toegangsmodifiers](#access-modifiers)
    - [Get en Set](#get-and-set)
    - [Auto-Accessors in Classes](#auto-accessors-in-classes)
    - [this](#this)
    - [Parameter-eigenschappen](#parameter-properties)
    - [Abstracte Classes](#abstract-classes)
    - [Met Generics](#with-generics)
    - [Decorators](#decorators)
      - [Class Decorators](#class-decorators)
      - [Property Decorator](#property-decorator)
      - [Method Decorator](#method-decorator)
      - [Getter en Setter Decorators](#getter-and-setter-decorators)
      - [Decorator Metadata](#decorator-metadata)
    - [Overerving](#inheritance)
    - [Statics](#statics)
    - [Eigenschapsinitialisatie](#property-initialization)
    - [Method Overloading](#method-overloading)
  - [Generics](#generics)
    - [Generiek Type](#generic-type)
    - [Generieke Classes](#generic-classes)
    - [Generieke Constraints](#generic-constraints)
    - [Generieke Contextuele Narrowing](#generic-contextual-narrowing)
  - [Erased Structural Types](#erased-structural-types)
  - [Namespacing](#namespacing)
  - [Symbols](#symbols)
  - [Triple-Slash Directives](#triple-slash-directives)
  - [Type Manipulatie](#type-manipulation)
    - [Types Maken van Types](#creating-types-from-types)
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
  - [Overige](#others)
    - [Fouten en Exception Handling](#errors-and-exception-handling)
    - [Mixin Classes](#mixin-classes)
    - [Asynchrone Taalfuncties](#asynchronous-language-features)
    - [Iterators en Generators](#iterators-and-generators)
    - [TsDocs JSDoc Referentie](#tsdocs-jsdoc-reference)
    - [@types](#types)
    - [JSX](#jsx-1)
    - [ES6 Modules](#es6-modules)
    - [ES7 Exponentiation Operator](#es7-exponentiation-operator)
    - [Het for-await-of Statement](#the-for-await-of-statement)
    - [Nieuwe target Meta-property](#new-target-meta-property)
    - [Dynamic Import Expressies](#dynamic-import-expressions)
    - ["tsc –watch"](#tsc-watch)
    - [Non-null Assertion Operator](#non-null-assertion-operator)
    - [Defaulted Declaraties](#defaulted-declarations)
    - [Optional Chaining](#optional-chaining)
    - [Nullish Coalescing Operator](#nullish-coalescing-operator)
    - [Template Literal Types](#template-literal-types)
    - [Functie Overloading](#function-overloading)
    - [Recursieve Types](#recursive-types)
    - [Recursieve Conditional Types](#recursive-conditional-types)
    - [ECMAScript Module Ondersteuning in Node](#ecmascript-module-support-in-node)
    - [Assertion Functions](#assertion-functions)
    - [Variadische Tuple Types](#variadic-tuple-types)
    - [Boxed Types](#boxed-types)
    - [Covariantie en Contravariantie in TypeScript](#covariance-and-contravariance-in-typescript)
      - [Optionele Variantie-annotaties voor Type Parameters](#optional-variance-annotations-for-type-parameters)
    - [Template String Pattern Index Signatures](#template-string-pattern-index-signatures)
    - [De satisfies Operator](#the-satisfies-operator)
    - [Type-Only Imports en Export](#type-only-imports-and-export)
    - [using Declaratie en Explicit Resource Management](#using-declaration-and-explicit-resource-management)
      - [await using Declaratie](#await-using-declaration)
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

TypeScript ondersteunt meerdere programmeerparadigma's, zoals functioneel, generiek, imperatief en objectgeoriënteerd. TypeScript is noch een geïnterpreteerde, noch een gecompileerde taal.

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

Het wordt aanbevolen om TypeScript projectmatig te installeren in plaats van globaal, omdat dit zorgt voor een voorspelbaarder bouwproces. Voor eenmalige gelegenheden kun je echter het volgende commando gebruiken:

```shell
npx tsc
```

of het globaal installeren:

```shell
npm install -g typescript
```

Als je Microsoft Visual Studio gebruikt, kun je TypeScript verkrijgen als een pakket in NuGet voor je MSBuild-projecten. Voer in de NuGet Package Manager Console het volgende commando uit:

```shell
Install-Package Microsoft.TypeScript.MSBuild
```

Tijdens de TypeScript-installatie worden twee uitvoerbare bestanden geïnstalleerd: "tsc" als de TypeScript-compiler en "tsserver" als de TypeScript standalone server. De standalone server bevat de compiler en taaldiensten die door editors en IDE's kunnen worden gebruikt om intelligente code-aanvulling (IntelliSense) te bieden.

Daarnaast zijn er verschillende TypeScript-compatibele transpilers beschikbaar, zoals Babel (via een plugin) of swc. Deze transpilers kunnen worden gebruikt om TypeScript-code om te zetten naar andere doeltalen of versies.

### Configuratie

TypeScript kan worden geconfigureerd met de tsc CLI-opties of door gebruik te maken van een speciaal configuratiebestand genaamd tsconfig.json, geplaatst in de root van het project.

Om een tsconfig.json-bestand te genereren dat vooraf is ingevuld met aanbevolen instellingen, kun je het volgende commando gebruiken:

```shell
tsc --init
```

Bij het lokaal uitvoeren van het `tsc` commando, zal TypeScript de code compileren met de configuratie die is gespecificeerd in het dichtstbijzijnde tsconfig.json bestand.

Hier zijn enkele voorbeelden van CLI-commando's die met de standaardinstellingen worden uitgevoerd:

```shell
tsc main.ts // Compileer een specifiek bestand (main.ts) naar JavaScript
tsc src/*.ts // Compileer alle .ts bestanden in de map 'src' naar JavaScript
tsc app.ts util.ts --outfile index.js // Compileer twee TypeScript-bestanden (app.ts en util.ts) naar één enkel JavaScript-bestand (index.js)
```

### TypeScript Configuratiebestand

Een tsconfig.json bestand wordt gebruikt om de TypeScript Compiler (tsc) te configureren. Meestal wordt het toegevoegd aan de root van het project, samen met het `package.json` bestand.

Opmerkingen:

* tsconfig.json accepteert commentaar, zelfs als het in JSON-formaat is.
* Het is raadzaam om dit configuratiebestand te gebruiken in plaats van de CLI-opties.

Op de volgende link vind je de volledige documentatie en het bijbehorende schema:

[https://www.typescriptlang.org/tsconfig](https://www.typescriptlang.org/tsconfig)

De volgende lijst bevat de meest voorkomende en nuttige configuraties:

#### target

De eigenschap "target" wordt gebruikt om te specificeren in welke versie van JavaScript (ECMAScript) je TypeScript moet compileren. Voor moderne browsers is ES6 een goede optie; voor oudere browsers wordt ES5 aanbevolen.

#### lib

De eigenschap "lib" wordt gebruikt om te specificeren welke bibliotheekbestanden moeten worden opgenomen tijdens de compilatie. TypeScript bevat automatisch API's voor functies die zijn gespecificeerd in de "target" eigenschap, maar het is mogelijk om specifieke bibliotheken weg te laten of te kiezen voor specifieke behoeften. Als je bijvoorbeeld aan een serverproject werkt, zou je de "DOM" bibliotheek kunnen uitsluiten, die alleen nuttig is in een browseromgeving.

#### strict

De eigenschap "strict" maakt sterkere garanties mogelijk en verhoogt de typeveiligheid. Het is raadzaam om deze eigenschap altijd op te nemen in het tsconfig.json bestand van je project. Het inschakelen van de "strict" eigenschap stelt TypeScript in staat om:

* Code te genereren met "use strict" voor elk bronbestand.
* "null" en "undefined" mee te nemen in het type-controleproces.
* Het gebruik van het "any" type uit te schakelen wanneer er geen type-annotaties aanwezig zijn.
* Een fout te genereren bij het gebruik van de "this" expressie, die anders het "any" type zou impliceren.

#### module

De eigenschap "module" stelt het modulesysteem in dat wordt ondersteund voor het gecompileerde programma. Tijdens runtime wordt een moduleloader gebruikt om afhankelijkheden te lokaliseren en uit te voeren op basis van het gespecificeerde modulesysteem.

De meest voorkomende moduleloaders die in JavaScript worden gebruikt, zijn Node.js CommonJS voor server-side applicaties en RequireJS voor AMD-modules in browser-gebaseerde webapplicaties. TypeScript kan code genereren voor verschillende modulesystemen, waaronder UMD, System, ESNext, ES2015/ES6 en ES2020.

Opmerking: Het modulesysteem moet worden gekozen op basis van de doelomgeving en het modulelaadmechanisme dat beschikbaar is in die omgeving.

#### moduleResolution

De eigenschap "moduleResolution" specificeert de strategie voor module-resolutie. Gebruik "node" voor moderne TypeScript-code; de "classic" strategie wordt alleen gebruikt voor oude versies van TypeScript (vóór 1.6).

#### esModuleInterop

De eigenschap "esModuleInterop" maakt het mogelijk om defaults te importeren uit CommonJS-modules die niet exporteerden met de "default" eigenschap. Deze eigenschap biedt een shim om compatibiliteit in de gegenereerde JavaScript te garanderen. Na het inschakelen van deze optie kunnen we `import MyLibrary from "my-library"` gebruiken in plaats van `import * as MyLibrary from "my-library"`.

#### jsx

De eigenschap "jsx" is alleen van toepassing op .tsx-bestanden die in ReactJS worden gebruikt en bepaalt hoe JSX-constructies naar JavaScript worden gecompileerd. Een veelvoorkomende optie is "preserve", die naar een .jsx-bestand compileert en de JSX ongewijzigd laat, zodat het kan worden doorgegeven aan andere tools zoals Babel voor verdere transformaties.

#### skipLibCheck

De eigenschap "skipLibCheck" voorkomt dat TypeScript de volledige geïmporteerde externe pakketten type-checkt. Deze eigenschap vermindert de compilatietijd van een project. TypeScript zal nog steeds je eigen code controleren tegen de typedefinities die door deze pakketten worden geleverd.

#### files

De eigenschap "files" geeft aan de compiler een lijst met bestanden door die altijd in het programma moeten worden opgenomen.

#### include

<!-- markdownlint-disable MD049 -->
De eigenschap "include" geeft aan de compiler een lijst met bestanden door die we willen opnemen. Deze eigenschap staat glob-achtige patronen toe, zoals "*" voor elke submap, "*" voor elke bestandsnaam en "?" voor optionele karakters.
<!-- markdownlint-enable MD049 -->

#### exclude

De eigenschap "exclude" geeft aan de compiler een lijst met bestanden door die niet in de compilatie moeten worden opgenomen. Dit kan bestanden bevatten zoals "node_modules" of testbestanden.
Opmerking: tsconfig.json staat commentaar toe.

### importHelpers

TypeScript gebruikt helper-code bij het genereren van code voor bepaalde geavanceerde of naar beneden gehaalde (down-leveled) JavaScript-functies. Standaard worden deze helpers gedupliceerd in bestanden die ze gebruiken. De `importHelpers` optie importeert deze helpers in plaats daarvan uit de `tslib` module, waardoor de JavaScript-output efficiënter wordt.

### Advies voor Migratie naar TypeScript

Voor grote projecten wordt aanbevolen om een geleidelijke overgang te maken waarbij TypeScript- en JavaScript-code in eerste instantie naast elkaar bestaan. Alleen kleine projecten kunnen in één keer naar TypeScript worden gemigreerd.

De eerste stap van deze overgang is het introduceren van TypeScript in het bouwproces. Dit kan worden gedaan door de compileroptie "allowJs" te gebruiken, die toestaat dat .ts en .tsx bestanden naast bestaande JavaScript-bestanden bestaan. Omdat TypeScript zal terugvallen op een type van "any" voor een variabele wanneer het het type niet kan afleiden uit JavaScript-bestanden, wordt aanbevolen om "noImplicitAny" uit te schakelen in je compileropties aan het begin van de migratie.

De tweede stap is ervoor zorgen dat je JavaScript-tests naast TypeScript-bestanden werken, zodat je tests kunt uitvoeren terwijl je elke module converteert. Als je Jest gebruikt, overweeg dan om `ts-jest` te gebruiken, waarmee je TypeScript-projecten met Jest kunt testen.

De derde stap is het opnemen van typedeclaraties voor externe bibliotheken in je project. Deze declaraties zijn ofwel gebundeld of te vinden op DefinitelyTyped. Je kunt naar ze zoeken via [https://www.typescriptlang.org/dt/search](https://www.typescriptlang.org/dt/search) en ze installeren met:

```shell
npm install --save-dev @types/pakket-naam
```

of

```shell
yarn add --dev @types/pakket-naam.
```

De vierde stap is om module voor module te migreren met een bottom-up benadering, waarbij je je afhankelijkheidsgraaf volgt beginnend bij de bladeren (leaves). Het idee is om te beginnen met het converteren van modules die niet afhankelijk zijn van andere modules. Om de afhankelijkheidsgrafen te visualiseren, kun je de tool "madge" gebruiken.

Goede kandidaten voor deze initiële conversies zijn utility-functies en code gerelateerd aan externe API's of specificaties. Het is mogelijk om automatisch TypeScript-typedefinities te genereren uit Swagger-contracten, GraphQL- of JSON-schema's om in je project op te nemen.

Wanneer er geen specificaties of officiële schema's beschikbaar zijn, kun je types genereren uit ruwe data, zoals JSON die door een server wordt geretourneerd. Het wordt echter aanbevolen om types te genereren uit specificaties in plaats van data om te voorkomen dat je randgevallen mist.

Onthoud je tijdens de migratie van code-refactoring en focus je alleen op het toevoegen van types aan je modules.

De vijfde stap is het inschakelen van "noImplicitAny", wat zal afdwingen dat alle types bekend en gedefinieerd zijn, wat een betere TypeScript-ervaring voor je project oplevert.

Tijdens de migratie kun je de `@ts-check` directive gebruiken, die TypeScript-typecontrole in een JavaScript-bestand inschakelt. Deze directive biedt een lossere versie van typecontrole en kan in het begin worden gebruikt om problemen in JavaScript-bestanden te identificeren. Wanneer `@ts-check` in een bestand is opgenomen, zal TypeScript proberen definities af te leiden met behulp van commentaar in JSDoc-stijl. Overweeg echter om JSDoc-annotaties alleen in een zeer vroeg stadium van de migratie te gebruiken.

Overweeg om de standaardwaarde van `noEmitOnError` in je tsconfig.json op false te houden. Dit stelt je in staat om JavaScript-broncode te genereren, zelfs als er fouten worden gerapporteerd.

## Het Typesysteem Verkennen

### De TypeScript Language Service

De TypeScript Language Service, ook wel bekend als tsserver, biedt verschillende functies zoals foutrapportage, diagnostiek, compile-on-save, hernoemen, ga naar definitie, aanvullingslijsten, handtekeninghulp en meer. Het wordt voornamelijk gebruikt door geïntegreerde ontwikkelomgevingen (IDE's) om IntelliSense-ondersteuning te bieden. Het integreert naadloos met Visual Studio Code en wordt gebruikt door tools zoals Conquer of Completion (Coc).

Ontwikkelaars kunnen gebruikmaken van een speciale API en hun eigen aangepaste language service plugins maken om de TypeScript-bewerkingservaring te verbeteren. Dit kan bijzonder nuttig zijn voor het implementeren van speciale linting-functies of het inschakelen van automatische aanvulling voor een aangepaste templating-taal.

<!-- markdownlint-disable MD044 -->
Een voorbeeld van een echte aangepaste plugin is "typescript-styled-plugin", die syntaxfoutrapportage en IntelliSense-ondersteuning biedt voor CSS-eigenschappen in styled components.
<!-- markdownlint-enable MD044 -->

Voor meer informatie en snelstartgidsen kun je de officiële TypeScript Wiki op GitHub raadplegen: [https://github.com/microsoft/TypeScript/wiki/](https://github.com/microsoft/TypeScript/wiki/)

### Structurele Typering

TypeScript is gebaseerd op een structureel typesysteem. Dit betekent dat de compatibiliteit en gelijkwaardigheid van types worden bepaald door de werkelijke structuur of definitie van het type, in plaats van de naam of de plaats van declaratie, zoals in nominatieve typesystemen zoals C# of C.

Het structurele typesysteem van TypeScript is ontworpen op basis van hoe JavaScript's dynamische "duck typing" systeem werkt tijdens runtime.

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

### Fundamentele Vergelijkingsregels van TypeScript

Het TypeScript-vergelijkingsproces is recursief en wordt uitgevoerd op types genest op elk niveau.

Een type "X" is compatibel met "Y" als "Y" ten minste dezelfde leden heeft als "X".

```typescript
type X = {
    a: string;
};
const y = { a: 'A', b: 'B' }; // Geldig, want het heeft ten minste dezelfde leden als X
const r: X = y;
```

Functieparameters worden vergeleken op basis van hun types, niet op basis van hun namen:

```typescript
type X = (a: number) => void;
type Y = (a: number) => void;
let x: X = (j: number) => undefined;
let y: Y = (k: number) => undefined;
y = x; // Geldig
x = y; // Geldig
```

Functie-return-types moeten hetzelfde zijn:

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
y = x; // Ongeldig, lid b ontbreekt
```

Het negeren van functieparameters is toegestaan, omdat dit een gangbare praktijk is in JavaScript, bijvoorbeeld bij het gebruik van "Array.prototype.map()":

```typescript
[1, 2, 3].map((element, _index, _array) => element + 'x');
```

Daarom zijn de volgende typedeclaraties volledig geldig:

```typescript
type X = (a: number) => undefined;
type Y = (a: number, b: number) => undefined;
let x: X = (a: number) => undefined;
let y: Y = (a: number) => undefined; // Ontbrekende b-parameter
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
let x: X = a => undefined; //geldig
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

Instanties van een klasse zijn onderworpen aan een compatibiliteitscontrole voor hun private en protected leden:

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

De vergelijkingscontrole houdt geen rekening met de verschillende overervingshiërarchie, bijvoorbeeld:

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

Generics worden vergeleken met hun structuren op basis van het resulterende type na toepassing van de generieke parameter; alleen het uiteindelijke resultaat wordt vergeleken als een niet-generiek type.

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

Wanneer generics hun type-argument niet gespecificeerd hebben, worden alle niet-gespecificeerde argumenten behandeld als types met "any":

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
g = 1; // Ongeldig, void is aan niets toewijsbaar behalve aan any
g = g1; // Geldig
```

Houd er rekening mee dat wanneer "strictNullChecks" is ingeschakeld, "null" en "undefined" vergelijkbaar worden behandeld als "void"; anders zijn ze vergelijkbaar met "never".

### Types als Verzamelingen

In TypeScript is een type een verzameling mogelijke waarden. Deze verzameling wordt ook wel het domein van het type genoemd. Elke waarde van een type kan worden gezien als een element in een verzameling. Een type stelt de beperkingen vast waaraan elk element in de verzameling moet voldoen om als lid van die verzameling te worden beschouwd.
De primaire taak van TypeScript is om te controleren en te verifiëren of de ene verzameling een deelverzameling (subset) is van de andere.

TypeScript ondersteunt verschillende soorten verzamelingen:

| Verzamelterm        | TypeScript                      | Opmerkingen                                                                                                        |
| ------------------- | ------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Lege verzameling    | never                           | "never" bevat niets behalve zichzelf                                                                               |
| Enkel-element-set   | undefined / null / literal type |                                                                                                                    |
| Eindige verzameling | boolean / union                 |                                                                                                                    |
| Oneindige verzam.   | string / number / object        |                                                                                                                    |
| Universele verzam.  | any / unknown                   | Elk element is lid van "any" en elke set is een deelverz. ervan / "unknown" is de typeveilige tegenhanger van "any" |

Hier zijn enkele voorbeelden:

| TypeScript            | Verzamelterm           | Voorbeeld                                                                       |
| --------------------- | ---------------------- | ------------------------------------------------------------------------------- |
| never                 | ∅ (lege verzameling)   | const x: never = 'x'; // Fout: Type 'string' is niet toewijsbaar aan type 'never' |
|                       |                        |
| Literal type          | Enkel-element-set      | type X = 'X';                                                                   |
|                       |                        | type Y = 7;                                                                     |
|                       |                        |
| Waarde toewijsbaar T  | Waarde ∈ T (lid van)   | type XY = 'X' \| 'Y';                                                           |
|                       |                        | const x: XY = 'X';                                                              |
|                       |                        |
| T1 toewijsbaar aan T2 | T1 ⊆ T2 (deelverz. van) | type XY = 'X' \| 'Y';                                                           |
|                       |                        | const x: XY = 'X';                                                              |
|                       |                        | const j: XY = 'J'; // Type '"J"' is niet toewijsbaar aan type 'XY'.             |
|                       |                        |                                                                                 |
| T1 extends T2         | T1 ⊆ T2 (deelverz. van) | type X = 'X' extends string ? true : false;                                     |
|                       |                        |
| T1 \| T2              | T1 ∪ T2 (unie)         | type XY = 'X' \| 'Y';                                                           |
|                       |                        | type JK = 1 \| 2;                                                               |
|                       |                        |
| T1 & T2               | T1 ∩ T2 (doorsnede)    | type X = \{ a: string \}                                                          |
|                       |                        | type Y = \{ b: string \}                                                          |
|                       |                        | type XY = X & Y                                                                 |
|                       |                        | const x: XY = \{ a: 'a', b: 'b' \}                                                |
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

Een doorsnede (T1 & T2) creëert een nauwere verzameling (alleen gedeeld):

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

Het trefwoord `extends` zou in deze context kunnen worden beschouwd als "deelverzameling van". Het stelt een beperking (constraint) in voor een type. De `extends` gebruikt bij een generic neemt de generic als een oneindige verzameling en zal deze beperken tot een specifieker type.
Houd er rekening mee dat `extends` niets te maken heeft met hiërarchie in de zin van OOP (dit concept bestaat niet in TypeScript).
TypeScript werkt met verzamelingen en heeft geen strikte hiërarchie; sterker nog, zoals in het onderstaande voorbeeld, kunnen twee types elkaar overlappen zonder dat de een een subtype van het andere type is (TypeScript kijkt naar de structuur, de vorm van de objecten).

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

### Een Type Toewijzen: Typedeclaraties en Type-assertions

Een type kan in TypeScript op verschillende manieren worden toegewezen:

#### Typedeclaratie

In het volgende voorbeeld gebruiken we x: X (": Type") om een type voor de variabele x te declareren.

```typescript
type X = {
    a: string;
};

// Typedeclaratie
const x: X = {
    a: 'a',
};
```

Als de variabele niet in het gespecificeerde formaat is, zal TypeScript een fout rapporteren. Bijvoorbeeld:

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

Het is mogelijk om een bewering (assertion) toe te voegen door het trefwoord `as` te gebruiken. Dit vertelt de compiler dat de ontwikkelaar meer informatie over een type heeft en onderdrukt eventuele fouten die kunnen optreden.

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

In het bovenstaande voorbeeld wordt beweerd dat het object x het type X heeft door gebruik te maken van het trefwoord `as`. Dit informeert de TypeScript-compiler dat het object voldoet aan het gespecificeerde type, ook al heeft het een extra eigenschap b die niet in de typedefinitie voorkomt.

Type-assertions zijn nuttig in situaties waarin een specifieker type moet worden opgegeven, vooral bij het werken met de DOM. Bijvoorbeeld:

```typescript
const myInput = document.getElementById('my_input') as HTMLInputElement;
```

Hier wordt de type-assertion `as HTMLInputElement` gebruikt om TypeScript te vertellen dat het resultaat van `getElementById` moet worden behandeld als een `HTMLInputElement`.
Type-assertions kunnen ook worden gebruikt om keys te hermappen (remap), zoals getoond in het onderstaande voorbeeld met template literals:

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

In dit voorbeeld gebruikt het type `J<Type>` een gemapt type met een template literal om de keys van `Type` te hermappen. Het creëert nieuwe eigenschappen met een toegevoegd "prefix_", en hun overeenkomstige waarden zijn functies die de oorspronkelijke eigenschapswaarden retourneren.

Het is vermeldenswaard dat bij het gebruik van een type-assertion TypeScript geen extra eigenschapscontrole (excess property checking) zal uitvoeren. Daarom is het over het algemeen verkieslijk om een typedeclaratie te gebruiken wanneer de structuur van het object vooraf bekend is.

#### Ambient Declarations

Ambient declarations zijn bestanden die types beschrijven voor JavaScript-code; ze hebben een bestandsnaamformaat als `.d.ts`. Ze worden meestal geïmporteerd en gebruikt om bestaande JavaScript-bibliotheken te annoteren of om types toe te voegen aan bestaande JS-bestanden in je project.

Veel types voor gangbare bibliotheken zijn te vinden op:
[https://github.com/DefinitelyTyped/DefinitelyTyped/](https://github.com/DefinitelyTyped/DefinitelyTyped/)

en kunnen worden geïnstalleerd met:

```shell
npm install --save-dev @types/bibliotheek-naam
```

Voor je eigen gedefinieerde Ambient Declarations kun je importeren met de "triple-slash" referentie:

<!-- skip -->
```typescript
/// <reference path="./library-types.d.ts" />
```

Je kunt Ambient Declarations zelfs gebruiken in JavaScript-bestanden met `// @ts-check`.

Het trefwoord `declare` maakt typedefinities mogelijk voor bestaande JavaScript-code zonder deze te importeren, en dient als een tijdelijke aanduiding voor types uit een ander bestand of globaal.

### Property Checking en Excess Property Checking

TypeScript is gebaseerd op een structureel typesysteem, maar excess property checking is een eigenschap van TypeScript die het in staat stelt te controleren of een object precies de eigenschappen heeft die in het type zijn gespecificeerd.

Excess Property Checking wordt uitgevoerd bij het toewijzen van object literals aan variabelen of bij het doorgeven ervan als argumenten aan de excess property van een functie, bijvoorbeeld.

<!-- skip -->
```typescript
type X = {
    a: string;
};
const y = { a: 'a', b: 'b' };
const x: X = y; // Geldig vanwege structurele typering
const w: X = { a: 'a', b: 'b' }; // Ongeldig vanwege excess property checking
```

### Weak Types

Een type wordt als zwak (weak) beschouwd wanneer het niets anders bevat dan een set van uitsluitend optionele eigenschappen:

```typescript
type X = {
    a?: string;
    b?: string;
};
```

TypeScript beschouwt het als een fout om iets toe te wijzen aan een zwak type wanneer er geen overlap is; het volgende geeft bijvoorbeeld een foutmelding:

<!-- skip -->
```typescript
type Options = {
    a?: string;
    b?: string;
};

const fn = (options: Options) => undefined;

fn({ c: 'c' }); // Ongeldig
```

Hoewel niet aanbevolen, is het indien nodig mogelijk om deze controle te omzeilen door gebruik te maken van een type-assertion:

```typescript
type Options = {
    a?: string;
    b?: string;
};
const fn = (options: Options) => undefined;
fn({ c: 'c' } as Options); // Geldig
```

Of door `unknown` toe te voegen aan de index-signature van het zwakke type:

```typescript
type Options = {
    [prop: string]: unknown;
    a?: string;
    b?: string;
};

const fn = (options: Options) => undefined;
fn({ c: 'c' }); // Geldig
```

### Strict Object Literal Checking (Freshness)

Strikte controle van object literals, ook wel "freshness" genoemd, is een functie in TypeScript die helpt bij het opsporen van overtollige of verkeerd gespelde eigenschappen die anders onopgemerkt zouden blijven in normale structurele type-controles.

Bij het maken van een object literal beschouwt de TypeScript-compiler deze als "vers" (fresh). Als de object literal wordt toegewezen aan een variabele of wordt doorgegeven als parameter, zal TypeScript een fout genereren als de object literal eigenschappen specificeert die niet bestaan in het doeltype.

"Freshness" verdwijnt echter wanneer een object literal wordt verbreed (widened) of wanneer een type-assertion wordt gebruikt.

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
fn(y); // Widening: Geen fouten, structureel type-compatibel

fn({ a: 'a', bx: 'b' }); // Freshness-controle: Ongeldig argument

let c: X = { a: 'a' };
let d: Y = { a: 'a', b: '' };
c = d; // Widening: Geen Freshness-controle
```

### Type Inference

TypeScript kan types afleiden wanneer er geen annotatie is opgegeven tijdens:

* Variabele-initialisatie.
* Lid-initialisatie.
* Het instellen van standaardwaarden voor parameters.
* Het return-type van een functie.

Bijvoorbeeld:

```typescript
let x = 'x'; // Het afgeleide type is string
```

De TypeScript-compiler analyseert de waarde of expressie en bepaalt het type op basis van de beschikbare informatie.

### Geavanceerdere Inferences

Wanneer meerdere expressies worden gebruikt bij type-inference, zoekt TypeScript naar de "beste gemeenschappelijke types". Bijvoorbeeld:

```typescript
let x = [1, 'x', 1, null]; // Het afgeleide type is: (string | number | null)[]
```

Als de compiler geen beste gemeenschappelijke types kan vinden, retourneert hij een unie-type. Bijvoorbeeld:

```typescript
let x = [new RegExp('x'), new Date()]; // Afgeleid type is: (RegExp | Date)[]
```

TypeScript maakt gebruik van "contextuele typering" op basis van de locatie van de variabele om types af te leiden. In het volgende voorbeeld weet de compiler dat `e` van het type `MouseEvent` is vanwege het `click` event-type dat is gedefinieerd in het lib.d.ts bestand, dat ambient declarations bevat voor verschillende gangbare JavaScript-constructies en de DOM:

```typescript
window.addEventListener('click', function (e) {}); // Het afgeleide type van e is MouseEvent
```

### Type Widening

Type widening is het proces waarbij TypeScript een type toewijst aan een variabele die is geïnitialiseerd zonder dat er een type-annotatie is opgegeven. Het staat nauwe tot bredere types toe, maar niet andersom.
In het volgende voorbeeld:

<!-- skip -->
```typescript
let x = 'x'; // TypeScript leidt string af, een breed type
let y: 'y' | 'x' = 'y'; // y types is een unie van literal types
y = x; // Ongeldig Type 'string' is niet toewijsbaar aan type '"x" | "y"'.
```

TypeScript wijst `string` toe aan `x` op basis van de enkele waarde die tijdens de initialisatie is opgegeven (`x`); dit is een voorbeeld van widening.

TypeScript biedt manieren om controle te hebben over het widening-proces, bijvoorbeeld door "const" te gebruiken.

### Const

Het gebruik van het trefwoord `const` bij het declareren van een variabele resulteert in een nauwere type-inference in TypeScript.

Bijvoorbeeld:

```typescript
const x = 'x'; // TypeScript leidt het type van x af als 'x', een nauwer type
let y: 'y' | 'x' = 'y';
y = x; // Geldig: Het type van x wordt afgeleid als 'x'
```

Door `const` te gebruiken om de variabele x te declareren, wordt het type vernauwd tot de specifieke literal waarde 'x'. Omdat het type van x is vernauwd, kan het zonder fouten aan de variabele y worden toegewezen.
De reden dat het type kan worden afgeleid, is dat `const` variabelen niet opnieuw kunnen worden toegewezen, zodat hun type kan worden vernauwd tot een specifiek literal type, in dit geval het literal type 'x'.

#### Const Modifier op Type Parameters

Vanaf versie 5.0 van TypeScript is het mogelijk om het `const` attribuut op een generieke type parameter te specificeren. Dit maakt het mogelijk om het meest nauwkeurige type te laten afleiden. Laten we een voorbeeld bekijken zonder het gebruik van `const`:

```typescript
function identity<T>(value: T) {
    // Geen const hier
    return value;
}
const values = identity({ a: 'a', b: 'b' }); // Afgeleid type is: { a: string; b: string; }
```

Zoals je kunt zien, worden de eigenschappen `a` and `b` afgeleid met een type van `string`.

Laten we nu het verschil zien met de `const` versie:

```typescript
function identity<const T>(value: T) {
    // Gebruik van const modifier op type parameters
    return value;
}
const values = identity({ a: 'a', b: 'b' }); // Afgeleid type is: { a: "a"; b: "b"; }
```

Nu kunnen we zien dat de eigenschappen `a` and `b` zijn afgeleid als `const`, dus `a` and `b` worden behandeld als string literals in plaats van alleen maar `string` types.

#### Const Assertion

Deze functie stelt je in staat om een variabele te declareren met een nauwkeuriger literal type op basis van de initialisatiewaarde, wat aan de compiler aangeeft dat de waarde moet worden behandeld als een onveranderlijke literal. Hier zijn enkele voorbeelden:

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

We kunnen specifiek zijn en een type doorgeven; in het volgende voorbeeld is eigenschap `x` van het type `number`:

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

### Type Narrowing

Type Narrowing is het proces in TypeScript waarbij een algemeen type wordt vernauwd tot een specifieker type. Dit gebeurt wanneer TypeScript de code analyseert en bepaalt dat bepaalde voorwaarden of bewerkingen de type-informatie kunnen verfijnen.

Het vernauwen van types kan op verschillende manieren gebeuren, waaronder:

#### Voorwaarden

Door gebruik te maken van voorwaardelijke statements, zoals `if` or `switch`, kan TypeScript het type vernauwen op basis van de uitkomst van de voorwaarde. Bijvoorbeeld:

```typescript
let x: number | undefined = 10;

if (x !== undefined) {
    x += 100; // Het type is number, dat was vernauwd door de voorwaarde
}
```

#### Throwing of Returning

Het gooien van een fout of het voortijdig terugkeren uit een aftakking kan worden gebruikt om TypeScript te helpen een type te vernauwen. Bijvoorbeeld:

```typescript
let x: number | undefined = 10;

if (x === undefined) {
    throw 'fout';
}
x += 100;
```

Andere manieren om types te vernauwen in TypeScript zijn:

* `instanceof` operator: Gebruikt om te controleren of een object een instantie is van een specifieke klasse.
* `in` operator: Gebruikt om te controleren of een eigenschap in een object bestaat.
* `typeof` operator: Gebruikt om het type van een waarde tijdens runtime te controleren.
* Ingebouwde functies zoals `Array.isArray()`: Gebruikt om te controleren of een waarde een array is.

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

In gevallen waarin TypeScript niet in staat is om een type te bepalen, is het mogelijk om een helperfunctie te schrijven die bekend staat als een "user-defined type guard". In het volgende voorbeeld zullen we een Type Predicate gebruiken om het type te vernauwen na het toepassen van een bepaalde filtering:

```typescript
const data = ['a', null, 'c', 'd', null, 'f'];

const r1 = data.filter(x => x != null); // Het type is (string | null)[], TypeScript was niet in staat om het type goed af te leiden

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

Strings kunnen over meerdere regels lopen als ze worden omgeven door het backtick (`) karakter:

```typescript
let sentence: string = `xxx,
   yyy`;
```

### boolean

Het datatype `boolean` in TypeScript slaat een binaire waarde op, ofwel `true` of `false`.

```typescript
const isReady: boolean = true;
```

### number

Een `number` datatype in TypeScript wordt vertegenwoordigd door een 64-bits floating-point waarde. Een `number` type kan zowel gehele getallen als breuken vertegenwoordigen.
TypeScript ondersteunt ook hexadecimaal, binair en octaal, bijvoorbeeld:

```typescript
const decimal: number = 10;
const hexadecimal: number = 0xa00d; // Hexadecimaal begint met 0x
const binary: number = 0b1010; // Binair begint met 0b
const octal: number = 0o633; // Octaal begint met 0o
```

### bigInt

Een `bigInt` vertegenwoordigt numerieke waarden die zeer groot zijn (groter dan 2^53 – 1) en niet kunnen worden vertegenwoordigd met een `number`.

Een `bigInt` kan worden gemaakt door de ingebouwde functie `BigInt()` aan te roepen of door `n` toe te voegen aan het einde van een integer numerieke literal:

```typescript
const x: bigint = BigInt(9007199254740991);
const y: bigint = 9007199254740991n;
```

Opmerkingen:

* `bigInt` waarden kunnen niet worden gemengd met `number` en kunnen niet worden gebruikt met de ingebouwde `Math` bibliotheek; ze moeten naar hetzelfde type worden omgezet.
* `bigInt` waarden zijn alleen beschikbaar als de target-configuratie ES2020 of hoger is.

### Symbol

Symbols zijn unieke identificatiekenmerken die kunnen worden gebruikt als eigenschaps-keys in objecten om naamconflicten te voorkomen.

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

De types `null` en `undefined` vertegenwoordigen beide geen waarde of de afwezigheid van enige waarde.

Het type `undefined` betekent dat de waarde niet is toegewezen of geïnitialiseerd, of duidt op een onbedoelde afwezigheid van een waarde.

Het type `null` betekent dat we weten dat het veld geen waarde heeft, dus de waarde is niet beschikbaar; het duidt op een opzettelijke afwezigheid van een waarde.

### Array

Een `array` is een datatype dat meerdere waarden van hetzelfde type (of niet) kan opslaan. Het kan worden gedefinieerd met de volgende syntaxis:

```typescript
const x: string[] = ['a', 'b'];
const y: Array<string> = ['a', 'b'];
const j: Array<string | number> = ['a', 1, 'b', 2]; // Unie
```

TypeScript ondersteunt alleen-lezen (readonly) arrays met de volgende syntaxis:

<!-- skip -->
```typescript
const x: readonly string[] = ['a', 'b']; // Readonly modifier
const y: ReadonlyArray<string> = ['a', 'b'];
const j: ReadonlyArray<string | number> = ['a', 1, 'b', 2];
j.push('x'); // Ongeldig
```

TypeScript ondersteunt tuples en readonly tuples:

```typescript
const x: [string, number] = ['a', 1];
const y: readonly [string, number] = ['a', 1];
```

### any

Het datatype `any` vertegenwoordigt letterlijk "elke" waarde; het is de standaardwaarde wanneer TypeScript het type niet kan afleiden of wanneer het niet is gespecificeerd.

Bij het gebruik van `any` slaat de TypeScript-compiler de typecontrole over, dus er is geen typeveiligheid wanneer `any` wordt gebruikt. Gebruik `any` over het algemeen niet om de compiler stil te houden wanneer er een fout optreedt; focus in plaats daarvan op het oplossen van de fout, aangezien het met `any` mogelijk is om contracten te verbreken en we de voordelen van TypeScript's autocomplete verliezen.

Het type `any` kan nuttig zijn tijdens een geleidelijke migratie van JavaScript naar TypeScript, omdat het de compiler kan stilhouden.

Gebruik voor nieuwe projecten de TypeScript-configuratie `noImplicitAny`, die TypeScript in staat stelt om fouten te melden waar `any` wordt gebruikt of afgeleid.

Het type `any` is meestal een bron van fouten die echte problemen met je types kunnen maskeren. Vermijd het gebruik ervan zoveel mogelijk.

## Type-annotaties

Bij variabelen die zijn gedeclareerd met `var`, `let` en `const`, is het mogelijk om optioneel een type toe te voegen:

```typescript
const x: number = 1;
```

TypeScript is goed in het afleiden van types, vooral bij eenvoudige types, dus deze declaraties zijn in de meeste gevallen niet nodig.

Bij functies is het mogelijk om type-annotaties toe te voegen aan parameters:

```typescript
function sum(a: number, b: number) {
    return a + b;
}
```

Het volgende is een voorbeeld met een anonieme functie (een zogenaamde lambda-functie):

```typescript
const sum = (a: number, b: number) => a + b;
```

Deze annotaties kunnen worden vermeden wanneer een standaardwaarde voor een parameter aanwezig is:

```typescript
const sum = (a = 10, b: number) => a + b;
```

Return-type annotaties kunnen aan functies worden toegevoegd:

```typescript
const sum = (a = 10, b: number): number => a + b;
```

Dit is vooral nuttig voor complexere functies, omdat het expliciet opschrijven van het return-type vóór een implementatie kan helpen om beter over de functie na te denken.

Overweeg over het algemeen om type-signaturen te annoteren, maar niet de lokale variabelen in de body, en voeg altijd types toe aan object literals.

## Optionele Eigenschappen

Een object kan optionele eigenschappen (Optional Properties) specificeren door een vraagteken `?` toe te voegen aan het einde van de eigenschapsnaam:

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

Het is mogelijk om schrijven naar een eigenschap te voorkomen door de modifier `readonly` te gebruiken, wat garandeert dat de eigenschap niet kan worden overschreven, maar geen garantie biedt voor totale onveranderlijkheid:

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

In TypeScript kunnen we `string`, `number` en `symbol` gebruiken als index-signature:

```typescript
type K = {
    [name: string | number]: string;
};
const k: K = { x: 'x', 1: 'b' };
console.log(k['x']);
console.log(k[1]);
console.log(k['1']); // Zelfde resultaat als k[1]
```

Houd er rekening mee dat JavaScript een index met `number` automatisch converteert naar een index met `string`, dus `k[1]` or `k["1"]` retourneren dezelfde waarde.

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

Het trefwoord `extends` werkt alleen op interfaces en klassen; gebruik voor types een doorsnede (intersection):

```typescript
type A = {
    a: number;
};
type B = {
    b: number;
};
type C = A & B;
```

Het is mogelijk om een type uit te breiden met behulp van een interface, maar niet andersom:

```typescript
type A = {
    a: string;
};
interface B extends A {
    b: string;
}
```

## Literal Types

Een Literal Type is een set van één element uit een collectief type; het definieert een zeer exacte waarde die een JavaScript-primitief is.

Literal Types in TypeScript zijn getallen, strings en booleans.

Voorbeeld van literals:

```typescript
const a = 'a'; // String literal type
const b = 1; // Numeriek literal type
const c = true; // Boolean literal type
```

String, numerieke en boolean Literal Types worden gebruikt in unies, type guards en type-aliases.
In het volgende voorbeeld zie je een type-alias unie; `O` kan alleen de gespecificeerde waarden zijn en geen andere string:

```typescript
type O = 'a' | 'b' | 'c';
```

## Literal Inference

Literal Inference is een functie in TypeScript waarmee het type van een variabele of parameter kan worden afgeleid op basis van zijn waarde.

In het volgende voorbeeld kunnen we zien dat TypeScript `x` beschouwt als een literal type omdat de waarde later niet meer kan worden gewijzigd, terwijl `y` wordt afgeleid als string omdat deze op elk later moment kan worden gewijzigd.

```typescript
const x = 'x'; // Literal type 'x', omdat deze waarde niet kan worden gewijzigd
let y = 'y'; // Type string, omdat we deze waarde kunnen wijzigen
```

In het volgende voorbeeld kunnen we zien dat `o.x` werd afgeleid als een `string` (en niet als een literal van `a`) omdat TypeScript ervan uitgaat dat de waarde op elk later moment kan worden gewijzigd.

<!-- skip -->
```typescript
type X = 'a' | 'b';

let o = {
    x: 'a', // Dit is een bredere string
};

const fn = (x: X) => `${x}-foo`;

console.log(fn(o.x)); // Argument van type 'string' is niet toewijsbaar aan parameter van type 'X'
```

Zoals je kunt zien, geeft de code een foutmelding bij het doorgeven van `o.x` aan `fn`, omdat X een nauwer type is.

We kunnen dit probleem oplossen door een type-assertion te gebruiken met `const` of het `X` type:

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

`strictNullChecks` is een TypeScript-compileroptie die strikte null-controle afdwingt. Wanneer deze optie is ingeschakeld, kunnen variabelen en parameters alleen worden toegewezen aan `null` of `undefined` als ze expliciet zijn gedeclareerd als dat type met behulp van het unie-type `null | undefined`. Als een variabele of parameter niet expliciet als nullable is gedeclareerd, zal TypeScript een fout genereren om potentiële runtime-fouten te voorkomen.

## Enums

In TypeScript is een `enum` een set benoemde constante waarden.

```typescript
enum Color {
    Red = '#ff0000',
    Green = '#00ff00',
    Blue = '#0000ff',
}
```

Enums kunnen op verschillende manieren worden gedefinieerd:

### Numerieke Enums

In TypeScript is een numerieke enum een enum waarbij aan elke constante een numerieke waarde wordt toegewezen, standaard beginnend bij 0.

```typescript
enum Size {
    Small, // waarde begint bij 0
    Medium,
    Large,
}
```

Het is mogelijk om aangepaste waarden te specificeren door ze expliciet toe te wijzen:

```typescript
enum Size {
    Small = 10,
    Medium,
    Large,
}
console.log(Size.Medium); // 11
```

### String Enums

In TypeScript is een string enum een enum waarbij aan elke constante een stringwaarde wordt toegewezen.

```typescript
enum Language {
    English = 'EN',
    Spanish = 'ES',
}
```

Opmerking: TypeScript staat het gebruik van heterogene enums toe waar string- en numerieke leden naast elkaar kunnen bestaan.

### Constante Enums

Een constante enum in TypeScript is een speciaal type enum waarvan alle waarden bekend zijn tijdens compilatie en overal waar de enum wordt gebruikt, worden "ingelined", wat resulteert in efficiëntere code.

```typescript
const enum Language {
    English = 'EN',
    Spanish = 'ES',
}
console.log(Language.English);
```

Wordt gecompileerd naar:

```typescript
console.log('EN' /* Language.English */);
```

Opmerkingen:
Const Enums hebben hardgecodeerde waarden waardoor de enum wordt gewist, wat efficiënter kan zijn in op zichzelf staande bibliotheken, maar over het algemeen niet wenselijk is. Ook kunnen Const Enums geen berekende leden hebben.

### Reverse Mapping

In TypeScript verwijst reverse mapping in enums naar de mogelijkheid om de naam van een enum-lid op te halen uit zijn waarde. Standaard hebben enum-leden forward mappings van naam naar waarde, maar reverse mappings kunnen worden gemaakt door expliciet waarden voor elk lid in te stellen. Reverse mappings zijn nuttig wanneer je een enum-lid wilt opzoeken op basis van zijn waarde, of wanneer je over alle enum-leden wilt itereren. Merk op dat alleen numerieke enum-leden reverse mappings genereren, terwijl string enum-leden helemaal geen reverse mapping krijgen.

De volgende enum:

```typescript
enum Grade {
    A = 90,
    B = 80,
    C = 70,
    F = 'fail',
}
```

Wordt gecompileerd naar:

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

### Ambient Enums

Een ambient enum in TypeScript is een type enum dat is gedefinieerd in een declaratiebestand (*.d.ts) zonder een bijbehorende implementatie. Het stelt je in staat om een set benoemde constanten te definiëren die op een typeveilige manier over verschillende bestanden kunnen worden gebruikt zonder de implementatiedetails in elk bestand te hoeven importeren.

### Berekende en Constante Leden

In TypeScript is een berekend lid (computed member) een lid van een enum dat een waarde heeft die tijdens runtime wordt berekend, terwijl een constant lid een lid is waarvan de waarde tijdens compilatie wordt ingesteld en tijdens runtime niet kan worden gewijzigd. Berekende leden zijn toegestaan in gewone enums, terwijl constante leden zijn toegestaan in zowel gewone als const enums.

```typescript
// Constante leden
enum Color {
    Red = 1,
    Green = 5,
    Blue = Red + Green,
}
console.log(Color.Blue); // 6 generatie tijdens compilatie
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

Enums worden aangeduid door unies die hun lid-types bevatten. De waarden van elk lid kunnen worden bepaald door constante of niet-constante expressies, waarbij leden met constante waarden literal types toegewezen krijgen. Ter illustratie: beschouw de declaratie van type E en zijn subtypes E.A, E.B en E.C. In dit geval vertegenwoordigt E de unie E.A | E.B | E.C.

```typescript
const identity = (value: number) => value;

enum E {
    A = 2 * 5, // Numerieke literal
    B = 'bar', // String literal
    C = identity(42), // Ondoorzichtig berekend
}

console.log(E.C); //42
```

## Narrowing

TypeScript narrowing is het proces van het verfijnen van het type van een variabele binnen een voorwaardelijk blok. Dit is nuttig bij het werken met unie-types, waarbij een variabele meer dan één type kan hebben.

TypeScript herkent verschillende manieren om het type te vernauwen:

### typeof Type Guards

De typeof type guard is een specifieke type guard in TypeScript die het type van een variabele controleert op basis van zijn ingebouwde JavaScript-type.

```typescript
const fn = (x: number | string) => {
    if (typeof x === 'number') {
        return x + 1; // x is number
    }
    return -1;
};
```

### Truthiness Narrowing

Truthiness narrowing in TypeScript werkt door te controleren of een variabele "truthy" of "falsy" is om zijn type dienovereenkomstig te vernauwen.

```typescript
const toUpperCase = (name: string | null) => {
    if (name) {
        return name.toUpperCase();
    } else {
        return null;
    }
};
```

### Equality Narrowing

Equality narrowing in TypeScript werkt door te controleren of een variabele gelijk is aan een specifieke waarde of niet, om zijn type dienovereenkomstig te vernauwen.

Het wordt gebruikt in combinatie met `switch` statements en vergelijkingsoperatoren zoals `===`, `!==`, `==`, and `!=` om types te vernauwen.

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

### In Operator Narrowing

De `in` operator narrowing in TypeScript is een manier om het type van een variabele te vernauwen op basis van het feit of een eigenschap binnen het type van de variabele bestaat.

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

### instanceof Narrowing

De `instanceof` operator narrowing in TypeScript is een manier om het type van een variabele te vernauwen op basis van zijn constructorfunctie, door te controleren of een object een instantie is van een bepaalde klasse of interface.

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

## Assignments

TypeScript narrowing met behulp van toewijzingen (assignments) is een manier om het type van een variabele te vernauwen op basis van de waarde die eraan is toegewezen. Wanneer een variabele een waarde krijgt toegewezen, leidt TypeScript zijn type af op basis van de toegewezen waarde en vernauwt het het type van de variabele om overeen te komen met het afgeleide type.

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

Control Flow Analysis in TypeScript is een manier om de codeflow statisch te analyseren om de types van variabelen af te leiden, waardoor de compiler de types van die variabelen naar behoefte kan vernauwen op basis van de resultaten van de analyse.

Vóór TypeScript 4.4 werd codeflow-analyse alleen toegepast op code binnen een if-statement, maar vanaf TypeScript 4.4 kan het ook worden toegepast op voorwaardelijke expressies en indirecte toegang tot discriminant-eigenschappen via const-variabelen.

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
        obj.foo; // Fout, geen narrowing omdat obj wordt toegewezen in de function body
    }
};
```

Opmerkingen: Tot vijf niveaus van indirectie worden geanalyseerd in voorwaardelijke expressies.

## Type Predicates

Type Predicates in TypeScript zijn functies die een boolean waarde retourneren en worden gebruikt om het type van een variabele naar een specifieker type te vernauwen.

```typescript
const isString = (value: unknown): value is string => typeof value === 'string';

const foo = (bar: unknown) => {
    if (isString(bar)) {
        console.log(bar.toUpperCase());
    } else {
        console.log('geen string');
    }
};
```

## Discriminated Unions

Discriminated Unions in TypeScript zijn een type unie-type dat een gemeenschappelijke eigenschap gebruikt, bekend als de discriminant, om de set mogelijke types voor de unie te vernauwen.

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

Wanneer een variabele wordt vernauwd tot een type dat geen waarden kan bevatten, zal de TypeScript-compiler afleiden dat de variabele van het `never` type moet zijn. Dit komt omdat het never type een waarde vertegenwoordigt die nooit geproduceerd kan worden.

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

## Exhaustiveness Checking

Exhaustiveness checking is een functie in TypeScript die garandeert dat alle mogelijke gevallen van een gediscrimineerde unie worden afgehandeld in een `switch` statement of een `if` statement.

```typescript
type Direction = 'up' | 'down';

const move = (direction: Direction) => {
    switch (direction) {
        case 'up':
            console.log('Omhoog bewegen');
            break;
        case 'down':
            console.log('Omlaag bewegen');
            break;
        default:
            const exhaustiveCheck: never = direction;
            console.log(exhaustiveCheck); // Deze regel zal nooit worden uitgevoerd
    }
};
```

Het `never` type wordt gebruikt om te garanderen dat de default-case uitputtend is en dat TypeScript een foutmelding geeft als er een nieuwe waarde wordt toegevoegd aan het Direction type zonder dat deze in het switch statement wordt afgehandeld.

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

Type-alias, vergelijkbaar met een interface, definieert de vorm van een object. Het kan echter ook een nieuw aangepast type maken dat is gebaseerd op een bestaand type of een combinatie van bestaande types. Dit omvat het definiëren van unie-types, intersectie-types en andere complexe types.

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
type Tuple3 = [a: T, T]; // Benoemde Tuple plus anonieme Tuple
```

## Vaste Lengte Tuple

Een Vaste Lengte Tuple is een specifiek type tuple dat een vast aantal elementen van specifieke types afdwingt en geen wijzigingen toestaat aan de lengte van de tuple zodra deze is gedefinieerd.

Vaste lengte tuples zijn nuttig wanneer je een verzameling waarden moet vertegenwoordigen met een specifiek aantal elementen en specifieke types, en je wilt garanderen dat de lengte en types van de tuple niet onbedoeld kunnen worden gewijzigd.

<!-- skip -->
```typescript
const x = [10, 'hello'] as const;
x.push(2); // Fout
```

## Union Type

Een Union Type is een type dat een waarde vertegenwoordigt die een van meerdere types kan zijn. Union Types worden aangeduid met het `|` symbool tussen elk mogelijk type.

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

type J = X & Y; // Intersection

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

Type van waarde in TypeScript verwijst naar de automatische afleiding van een type uit een waarde of expressie door middel van type-inference.

```typescript
const x = 'x'; // TypeScript leidt 'x' af als een string literal met 'const' (onveranderlijk), maar verbreedt het tot 'string' met 'let' (opnieuw toewijsbaar).
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
const r = add(1, 2); // r is number
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

## infer Type Inference in Conditional Types

Het trefwoord `infer` wordt gebruikt in conditional types om het type van een generieke parameter af te leiden (te extraheren) uit een type dat ervan afhankelijk is. Hierdoor kun je flexibelere en herbruikbare typedefinities schrijven.

```typescript
type ElementType<T> = T extends (infer U)[] ? U : never;
type Numbers = ElementType<number[]>; // number
type Strings = ElementType<string[]>; // string
```

## Vooraf Gedefinieerde Conditional Types

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

Het type `any` is een speciaal type (universeel supertype) dat kan worden gebruikt om elk type waarde te vertegenwoordigen (primitieven, objecten, arrays, functies, fouten, symbols). Het wordt vaak gebruikt in situaties waarin het type van een waarde niet bekend is tijdens compilatie, of bij het werken met waarden uit externe API's of bibliotheken die geen TypeScript-typings hebben.

Door het type `any` te gebruiken, geef je aan de TypeScript-compiler aan dat waarden zonder enige beperking moeten worden weergegeven. Overweeg het volgende om de typeveiligheid in je code te maximaliseren:

* Beperk het gebruik van `any` tot specifieke gevallen waarin het type werkelijk onbekend is.
* Retourneer geen `any` types uit een functie, omdat je de typeveiligheid verliest in de code die die functie gebruikt, wat je typeveiligheid verzwakt.
* Gebruik in plaats van `any` `@ts-ignore` als je de compiler stil moet houden.

```typescript
let value: any;
value = true; // Geldig
value = 7; // Geldig
```

## Unknown type

In TypeScript vertegenwoordigt het type `unknown` een waarde waarvan het type onbekend is. In tegenstelling tot het type `any`, dat elk type waarde toestaat, vereist `unknown` een typecontrole of assertion voordat het op een specifieke manier kan worden gebruikt, dus er zijn geen bewerkingen toegestaan op een `unknown` zonder eerst te beweren of te vernauwen naar een specifieker type.

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

Het type `never` vertegenwoordigt waarden die nooit voorkomen. Het wordt gebruikt om functies of expressies aan te duiden die nooit iets retourneren of een fout gooien.

Bijvoorbeeld een oneindige loop:

```typescript
const infiniteLoop = (): never => {
    while (true) {
        // doe iets
    }
};
```

Het gooien van een fout:

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


## Interface en Type

### Gemeenschappelijke Syntaxis

In TypeScript definiëren interfaces de structuur van objecten, waarbij de namen en types van eigenschappen of methoden die een object moet hebben worden gespecificeerd. De gemeenschappelijke syntaxis voor het definiëren van een interface in TypeScript is als volgt:

<!-- skip -->
```typescript
interface InterfaceName {
    property1: Type1;
    // ...
    method1(arg1: ArgType1, arg2: ArgType2): ReturnType;
    // ...
}
```

Op vergelijkbare wijze voor een typedefinitie:

<!-- skip -->
```typescript
type TypeName = {
    property1: Type1;
    // ...
    method1(arg1: ArgType1, arg2: ArgType2): ReturnType;
    // ...
};
```

`interface InterfaceName` of `type TypeName`: Definieert de naam van de interface.
`property1`: `Type1`: Specificeert de eigenschappen van de interface samen met hun overeenkomstige types. Meerdere eigenschappen kunnen worden gedefinieerd, elk gescheiden door een puntkomma.
`method1(arg1: ArgType1, arg2: ArgType2): ReturnType;`: Specificeert de methoden van de interface. Methoden worden gedefinieerd met hun namen, gevolgd door een parameterlijst tussen haakjes en het return-type. Meerdere methoden kunnen worden gedefinieerd, elk gescheiden door een puntkomma.

Voorbeeld van een interface:

```typescript
interface Person {
    name: string;
    age: number;
    greet(): void;
}
```

Voorbeeld van een type:

```typescript
type TypeName = {
    property1: string;
    method1(arg1: string, arg2: string): string;
};
```

In TypeScript worden types gebruikt om de vorm van gegevens te definiëren en typecontrole af te dwingen. Er zijn verschillende gemeenschappelijke syntaxen voor het definiëren van types in TypeScript, afhankelijk van het specifieke gebruiksgeval. Hier zijn enkele voorbeelden:

### Basis Types

```typescript
let myNumber: number = 123; // number type
let myBoolean: boolean = true; // boolean type
let myArray: string[] = ['a', 'b']; // array van strings
let myTuple: [string, number] = ['a', 123]; // tuple
```

### Objecten en Interfaces

```typescript
const x: { name: string; age: number } = { name: 'Simon', age: 7 };
```

### Union en Intersection Types

```typescript
type MyType = string | number; // Union type
let myUnion: MyType = 'hello'; // Kan een string zijn
myUnion = 123; // Of een getal

type TypeA = { name: string };
type TypeB = { age: number };
type CombinedType = TypeA & TypeB; // Intersection type
let myCombined: CombinedType = { name: 'John', age: 25 }; // Object met zowel name als age eigenschappen
```

## Ingebouwde Type Primitieven

TypeScript heeft verschillende ingebouwde type primitieven die kunnen worden gebruikt om variabelen, functieparameters en return-types te definiëren:

* `number`: Vertegenwoordigt numerieke waarden, inclusief gehele getallen en zwevendekommagetallen.
* `string`: Vertegenwoordigt tekstuele gegevens.
* `boolean`: Vertegenwoordigt logische waarden, die true of false kunnen zijn.
* `null`: Vertegenwoordigt de afwezigheid van een waarde.
* `undefined`: Vertegenwoordigt een waarde die niet is toegewezen of niet is gedefinieerd.
* `symbol`: Vertegenwoordigt een unieke identificatie. Symbols worden doorgaans gebruikt als keys voor objecteigenschappen.
* `bigint`: Vertegenwoordigt gehele getallen met willekeurige precisie.
* `any`: Vertegenwoordigt een dynamisch of onbekend type. Variabelen van het type any kunnen waarden van elk type bevatten en ze omzeilen de typecontrole.
* `void`: Vertegenwoordigt de afwezigheid van enig type. Het wordt veel gebruikt als het return-type van functies die geen waarde retourneren.
* `never`: Vertegenwoordigt een type voor waarden die nooit voorkomen. Het wordt doorgaans gebruikt als het return-type van functies die een fout gooien of in een oneindige loop terechtkomen.

## Veelvoorkomende Ingebouwde JS Objecten

TypeScript is een superset van JavaScript en bevat alle veelgebruikte ingebouwde JavaScript-objecten. Je kunt een uitgebreide lijst van deze objecten vinden op de Mozilla Developer Network (MDN) documentatie-website:
[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)

Hier is een lijst van enkele veelgebruikte ingebouwde JavaScript-objecten:

* Function
* Object
* Boolean
* Error
* Number
* BigInt
* Math
* Date
* String
* RegExp
* Array
* Map
* Set
* Promise
* Intl

## Overloads

Functie-overloads in TypeScript stellen je in staat om meerdere functiesignaturen te definiëren voor een enkele functienaam, waardoor je functies kunt definiëren die op meerdere manieren kunnen worden aangeroepen. Hier is een voorbeeld:

```typescript
// Overloads
function sayHi(name: string): string;
function sayHi(names: string[]): string[];

// Implementatie
function sayHi(name: unknown): unknown {
    if (typeof name === 'string') {
        return `Hi, ${name}!`;
    } else if (Array.isArray(name)) {
        return name.map(name => `Hi, ${name}!`);
    }
    throw new Error('Invalid value');
}

sayHi('xx'); // Geldig
sayHi(['aa', 'bb']); // Geldig
```

Hier is nog een voorbeeld van het gebruik van functie-overloads binnen een `class`:

```typescript
class Greeter {
    message: string;

    constructor(message: string) {
        this.message = message;
    }

    // overload
    sayHi(name: string): string;
    sayHi(names: string[]): ReadonlyArray<string>;

    // implementatie
    sayHi(name: unknown): unknown {
        if (typeof name === 'string') {
            return `${this.message}, ${name}!`;
        } else if (Array.isArray(name)) {
            return name.map(name => `${this.message}, ${name}!`);
        }
        throw new Error('value is invalid');
    }
}
console.log(new Greeter('Hello').sayHi('Simon'));
```

## Samenvoegen en Uitbreiden

Samenvoegen (merging) en uitbreiden (extension) verwijzen naar twee verschillende concepten gerelateerd aan het werken met types en interfaces.

Samenvoegen stelt je in staat om meerdere declaraties met dezelfde naam te combineren tot een enkele definitie, bijvoorbeeld wanneer je een interface met dezelfde naam meerdere keren definieert:

```typescript
interface X {
    a: string;
}

interface X {
    b: number;
}

const person: X = {
    a: 'a',
    b: 7,
};
```

Uitbreiden verwijst naar de mogelijkheid om bestaande types of interfaces uit te breiden of ervan over te erven om nieuwe te creëren. Het is een mechanisme om extra eigenschappen of methoden aan een bestaand type toe te voegen zonder de oorspronkelijke definitie te wijzigen. Voorbeeld:

```typescript
interface Animal {
    name: string;
    eat(): void;
}

interface Bird extends Animal {
    sing(): void;
}

const dog: Bird = {
    name: 'Bird 1',
    eat() {
        console.log('Eating');
    },
    sing() {
        console.log('Singing');
    },
};
```

## Verschillen tussen Type en Interface

Declaratie samenvoeging (augmentation):

Interfaces ondersteunen declaratie samenvoeging, wat betekent dat je meerdere interfaces met dezelfde naam kunt definiëren, en TypeScript zal ze samenvoegen tot een enkele interface met de gecombineerde eigenschappen en methoden. Aan de andere kant ondersteunen types geen declaratie samenvoeging. Dit kan nuttig zijn wanneer je extra functionaliteit wilt toevoegen of bestaande types wilt aanpassen zonder de oorspronkelijke definities te wijzigen of ontbrekende of onjuiste types aan te vullen.

```typescript
interface A {
    x: string;
}
interface A {
    y: string;
}
const j: A = {
    x: 'xx',
    y: 'yy',
};
```

Het uitbreiden van andere types/interfaces:

Zowel types als interfaces kunnen andere types/interfaces uitbreiden, maar de syntaxis is anders. Bij interfaces gebruik je het trefwoord `extends` om eigenschappen en methoden over te erven van andere interfaces. Een interface kan echter geen complex type zoals een unie-type uitbreiden.

```typescript
interface A {
    x: string;
    y: number;
}
interface B extends A {
    z: string;
}
const car: B = {
    x: 'x',
    y: 123,
    z: 'z',
};
```

Voor types gebruik je de `&` operator om meerdere types te combineren tot een enkel type (intersection).

```typescript
interface A {
    x: string;
    y: number;
}

type B = A & {
    j: string;
};

const c: B = {
    x: 'x',
    y: 123,
    j: 'j',
};
```

Union en Intersection Types:

Types zijn flexibeler als het gaat om het definiëren van Union en Intersection Types. Met het trefwoord `type` kun je eenvoudig unie-types maken met de `|` operator en intersectie-types met de `&` operator. Hoewel interfaces ook indirect unie-types kunnen vertegenwoordigen, hebben ze geen ingebouwde ondersteuning voor intersectie-types.

```typescript
type Department = 'dep-x' | 'dep-y'; // Union

type Person = {
    name: string;
    age: number;
};

type Employee = {
    id: number;
    department: Department;
};

type EmployeeInfo = Person & Employee; // Intersection
```

Voorbeeld met interfaces:

```typescript
interface A {
    x: 'x';
}
interface B {
    y: 'y';
}

type C = A | B; // Unie van interfaces
```

## Class

### Algemene Class Syntaxis

Het trefwoord `class` wordt in TypeScript gebruikt om een klasse te definiëren. Hieronder zie je een voorbeeld:

```typescript
class Person {
    private name: string;
    private age: number;
    constructor(name: string, age: number) {
        this.name = name;
        this.age = age;
    }
    public sayHi(): void {
        console.log(
            `Hello, my name is ${this.name} and I am ${this.age} years old.`
        );
    }
}
```

Het trefwoord `class` wordt gebruikt om een klasse genaamd "Person" te definiëren.

De klasse heeft twee private eigenschappen: name van het type `string` en age van het type `number`.

De constructor wordt gedefinieerd met het trefwoord `constructor`. Deze accepteert name en age als parameters en wijst ze toe aan de overeenkomstige eigenschappen.

De klasse heeft een `public` methode genaamd sayHi die een begroeting logt.

Om een instantie van een klasse te maken in TypeScript, gebruik je het trefwoord `new` gevolgd door de klassenaam en haakjes `()`. Bijvoorbeeld:

<!-- skip -->
```typescript
const myObject = new Person('John Doe', 25);
myObject.sayHi(); // Output: Hello, my name is John Doe and I am 25 years old.
```

### Constructor

Constructoren zijn speciale methoden binnen een klasse die worden gebruikt om de eigenschappen van het object te initialiseren wanneer een instantie van de klasse wordt gemaakt.

```typescript
class Person {
    public name: string;
    public age: number;

    constructor(name: string, age: number) {
        this.name = name;
        this.age = age;
    }

    sayHello() {
        console.log(
            `Hello, my name is ${this.name} and I'm ${this.age} years old.`
        );
    }
}

const john = new Person('Simon', 17);
john.sayHello();
```

Het is mogelijk om een constructor te overloaden met de volgende syntaxis:

```typescript
type Sex = 'm' | 'f';

class Person {
    name: string;
    age: number;
    sex: Sex;

    constructor(name: string, age: number, sex?: Sex);
    constructor(name: string, age: number, sex: Sex) {
        this.name = name;
        this.age = age;
        this.sex = sex ?? 'm';
    }
}

const p1 = new Person('Simon', 17);
const p2 = new Person('Alice', 22, 'f');
```

In TypeScript is het mogelijk om meerdere constructor-overloads te definiëren, maar je kunt slechts één implementatie hebben die compatibel moet zijn met alle overloads; dit kan worden bereikt door een optionele parameter te gebruiken.

```typescript
class Person {
    name: string;
    age: number;

    constructor();
    constructor(name: string);
    constructor(name: string, age: number);
    constructor(name?: string, age?: number) {
        this.name = name ?? 'Unknown';
        this.age = age ?? 0;
    }

    displayInfo() {
        console.log(`Name: ${this.name}, Age: ${this.age}`);
    }
}

const person1 = new Person();
person1.displayInfo(); // Name: Unknown, Age: 0

const person2 = new Person('John');
person2.displayInfo(); // Name: John, Age: 0

const person3 = new Person('Jane', 25);
person3.displayInfo(); // Name: Jane, Age: 25
```

### Private en Protected Constructoren

In TypeScript kunnen constructoren worden gemarkeerd als private of protected, wat hun toegankelijkheid en gebruik beperkt.

Private Constructoren:
Kunnen alleen binnen de klasse zelf worden aangeroepen. Private constructoren worden vaak gebruikt in scenario's waarin je een singleton-patroon wilt afdwingen of het maken van instanties wilt beperken tot een factory-methode binnen de klasse.

Protected Constructoren:
Protected constructoren zijn nuttig wanneer je een basisklasse wilt maken die niet direct geïnstantieerd mag worden, maar wel kan worden uitgebreid door subklassen.

```typescript
class BaseClass {
    protected constructor() {}
}

class DerivedClass extends BaseClass {
    private value: number;

    constructor(value: number) {
        super();
        this.value = value;
    }
}

// Poging om de basisklasse direct te instantiëren zal een fout opleveren
// const baseObj = new BaseClass(); // Fout: Constructor of class 'BaseClass' is protected.

// Maak een instantie van de afgeleide klasse
const derivedObj = new DerivedClass(10);
```

### Toegangsmodifiers

Toegangsmodifiers `private`, `protected` en `public` worden gebruikt om de zichtbaarheid en toegankelijkheid van klasseleden, zoals eigenschappen en methoden, in TypeScript-klassen te regelen. Deze modifiers zijn essentieel voor het afdwingen van inkapseling (encapsulation) en het vaststellen van grenzen voor het benaderen en wijzigen van de interne status van een klasse.

De `private` modifier beperkt de toegang tot het klasseelement tot alleen binnen de bevattende klasse.

De `protected` modifier staat toegang tot het klasseelement toe binnen de bevattende klasse en de daarvan afgeleide klassen.

De `public` modifier biedt onbeperkte toegang tot het klasseelement, waardoor het overal vandaan kan worden benaderd.

### Get en Set

Getters en setters zijn speciale methoden waarmee je aangepast toegangs- en wijzigingsgedrag voor klasse-eigenschappen kunt definiëren. Ze stellen je in staat om de interne status van een object in te kapselen en extra logica te bieden bij het ophalen of instellen van de waarden van eigenschappen.
In TypeScript worden getters en setters gedefinieerd met respectievelijk de trefwoorden `get` and `set`. Hier is een voorbeeld:

```typescript
class MyClass {
    private _myProperty: string;

    constructor(value: string) {
        this._myProperty = value;
    }
    get myProperty(): string {
        return this._myProperty;
    }
    set myProperty(value: string) {
        this._myProperty = value;
    }
}
```

### Auto-Accessors in Classes

TypeScript versie 4.9 voegt ondersteuning toe voor auto-accessors, een toekomstige ECMAScript-functie. Ze lijken op klasse-eigenschappen maar worden gedeclareerd met het trefwoord "accessor".

```typescript
class Animal {
    accessor name: string;

    constructor(name: string) {
        this.name = name;
    }
}
```

Auto-accessors worden "omgezet" (de-sugared) naar private `get` en `set` accessors, die werken op een ontoegankelijke eigenschap.

<!-- skip -->
```typescript
class Animal {
    #__name: string;

    get name() {
        return this.#__name;
    }
    set name(value: string) {
        this.#__name = name;
    }

    constructor(name: string) {
        this.name = name;
    }
}
```

### this

In TypeScript verwijst het trefwoord `this` naar de huidige instantie van een klasse binnen zijn methoden of constructoren. Het stelt je in staat om de eigenschappen en methoden van de klasse te benaderen en te wijzigen vanuit zijn eigen scope.
Het biedt een manier om de interne status van een object te benaderen en te manipuleren binnen zijn eigen methoden.

```typescript
class Person {
    private name: string;
    constructor(name: string) {
        this.name = name;
    }
    public introduce(): void {
        console.log(`Hello, my name is ${this.name}.`);
    }
}

const person1 = new Person('Alice');
person1.introduce(); // Hello, my name is Alice.
```

### Parameter-eigenschappen

Parameter-eigenschappen (parameter properties) stellen je in staat om klasse-eigenschappen direct binnen de constructorparameters te declareren en te initialiseren, waardoor boilerplate-code wordt vermeden. Voorbeeld:

```typescript
class Person {
    constructor(
        private name: string,
        public age: number
    ) {
        // De trefwoorden "private" en "public" in de constructor
        // declareren en initialiseren automatisch de bijbehorende klasse-eigenschappen.
    }
    public introduce(): void {
        console.log(
            `Hello, my name is ${this.name} and I am ${this.age} years old.`
        );
    }
}
const person = new Person('Alice', 25);
person.introduce();
```

### Abstracte Classes

Abstracte klassen worden in TypeScript voornamelijk gebruikt voor overerving; ze bieden een manier om gemeenschappelijke eigenschappen en methoden te definiëren die door subklassen kunnen worden overgeërfd.
Dit is nuttig wanneer je gemeenschappelijk gedrag wilt definiëren en wilt afdwingen dat subklassen bepaalde methoden implementeren. Ze bieden een manier om een hiërarchie van klassen te creëren waarbij de abstracte basisklasse een gedeelde interface en gemeenschappelijke functionaliteit voor de subklassen biedt.

```typescript
abstract class Animal {
    protected name: string;

    constructor(name: string) {
        this.name = name;
    }

    abstract makeSound(): void;
}

class Cat extends Animal {
    makeSound(): void {
        console.log(`${this.name} meows.`);
    }
}

const cat = new Cat('Whiskers');
cat.makeSound(); // Output: Whiskers meows.
```

### Met Generics

Klassen met generics stellen je in staat om herbruikbare klassen te definiëren die met verschillende types kunnen werken.

```typescript
class Container<T> {
    private item: T;

    constructor(item: T) {
        this.item = item;
    }

    getItem(): T {
        return this.item;
    }

    setItem(item: T): void {
        this.item = item;
    }
}

const container1 = new Container<number>(42);
console.log(container1.getItem()); //  42

const container2 = new Container<string>('Hello');
container2.setItem('World');
console.log(container2.getItem()); // World
```

### Decorators

Decorators bieden een mechanisme om metadata toe te voegen, gedrag te wijzigen, te valideren of de functionaliteit van het doelelement uit te breiden. Het zijn functies die tijdens runtime worden uitgevoerd. Er kunnen meerdere decorators op een declaratie worden toegepast.

Decorators zijn experimentele functies en de volgende voorbeelden zijn alleen compatibel met TypeScript versie 5 of hoger met ES6.

Voor TypeScript-versies vóór 5 moeten ze worden ingeschakeld met de eigenschap `experimentalDecorators` in je `tsconfig.json` of door `–experimentalDecorators` te gebruiken in je opdrachtregel (maar het volgende voorbeeld zal dan niet werken).

Enkele veelvoorkomende gebruiksgevallen voor decorators zijn:

* Het observeren van eigenschapswijzigingen.
* Het observeren van methode-aanroepen.
* Het toevoegen van extra eigenschappen of methoden.
* Runtime-validatie.
* Automatische serialisatie en deserialisatie.
* Logging.
* Autorisatie en authenticatie.
* Foutafhandeling (error guarding).

Opmerking: Decorators voor versie 5 staan het decoreren van parameters niet toe.

Typen decorators:

#### Class Decorators

Class Decorators zijn nuttig voor het uitbreiden van een bestaande klasse, zoals het toevoegen van eigenschappen of methoden, of het verzamelen van instanties van een klasse. In het volgende voorbeeld voegen we een `toString` methode toe die de klasse omzet in een stringrepresentatie.

```typescript
type Constructor<T = {}> = new (...args: any[]) => T;

function toString<Class extends Constructor>(
    Value: Class,
    context: ClassDecoratorContext<Class>
) {
    return class extends Value {
        constructor(...args: any[]) {
            super(...args);
            console.log(JSON.stringify(this));
            console.log(JSON.stringify(context));
        }
    };
}

@toString
class Person {
    name: string;

    constructor(name: string) {
        this.name = name;
    }

    greet() {
        return 'Hello, ' + this.name;
    }
}
const person = new Person('Simon');
/* Logs:
{"name":"Simon"}
{"kind":"class","name":"Person"}
*/
```

#### Property Decorator

Property decorators zijn nuttig voor het wijzigen van het gedrag van een eigenschap, zoals het wijzigen van de initialisatiewaarden. In de volgende code hebben we een script dat een eigenschap instelt om altijd in hoofdletters te staan:

```typescript
function upperCase<T>(
    target: undefined,
    context: ClassFieldDecoratorContext<T, string>
) {
    return function (this: T, value: string) {
        return value.toUpperCase();
    };
}

class MyClass {
    @upperCase
    prop1 = 'hello!';
}

console.log(new MyClass().prop1); // Logs: HELLO!
```

#### Method Decorator

Method decorators stellen je in staat om het gedrag van methoden te wijzigen of te verbeteren. Hieronder staat een voorbeeld van een eenvoudige logger:

```typescript
function log<This, Args extends any[], Return>(
    target: (this: This, ...args: Args) => Return,
    context: ClassMethodDecoratorContext<
        This,
        (this: This, ...args: Args) => Return
    >
) {
    const methodName = String(context.name);

    function replacementMethod(this: This, ...args: Args): Return {
        console.log(`LOG: Entering method '${methodName}'.`);
        const result = target.call(this, ...args);
        console.log(`LOG: Exiting method '${methodName}'.`);
        return result;
    }

    return replacementMethod;
}

class MyClass {
    @log
    sayHello() {
        console.log('Hello!');
    }
}

new MyClass().sayHello();
```

Het logt:

```shell
LOG: Entering method 'sayHello'.
Hello!
LOG: Exiting method 'sayHello'.
```

#### Getter en Setter Decorators

Getter en setter decorators stellen je in staat om het gedrag van klasse-accessors te wijzigen of te verbeteren. Ze zijn bijvoorbeeld nuttig voor het valideren van eigenschapstoewijzingen. Hier is een eenvoudig voorbeeld voor een getter decorator:

```typescript
function range<This, Return extends number>(min: number, max: number) {
    return function (
        target: (this: This) => Return,
        context: ClassGetterDecoratorContext<This, Return>
    ) {
        return function (this: This): Return {
            const value = target.call(this);
            if (value < min || value > max) {
                throw 'Invalid';
            }
            Object.defineProperty(this, context.name, {
                value,
                enumerable: true,
            });
            return value;
        };
    };
}

class MyClass {
    private _value = 0;

    constructor(value: number) {
        this._value = value;
    }
    @range(1, 100)
    get getValue(): number {
        return this._value;
    }
}

const obj = new MyClass(10);
console.log(obj.getValue); // Geldig: 10

const obj2 = new MyClass(999);
console.log(obj2.getValue); // Gooit fout: Invalid!
```

#### Decorator Metadata

Decorator Metadata vereenvoudigt het proces voor decorators om metadata toe te passen en te gebruiken in elke klasse. Ze hebben toegang tot een nieuwe metadata-eigenschap op het context-object, die kan dienen als key voor zowel primitieven als objecten.
Metadata-informatie kan op de klasse worden benaderd via `Symbol.metadata`.

Metadata kan voor verschillende doeleinden worden gebruikt, zoals debugging, serialisatie of dependency injection met decorators.

```typescript
//@ts-ignore
Symbol.metadata ??= Symbol('Symbol.metadata'); // Eenvoudige polyfill

type Context =
    | ClassFieldDecoratorContext
    | ClassAccessorDecoratorContext
    | ClassMethodDecoratorContext; // Context bevat property metadata: DecoratorMetadata

function setMetadata(_target: any, context: Context) {
    // Stel het metadata-object in met een primitieve waarde
    context.metadata[context.name] = true;
}

class MyClass {
    @setMetadata
    a = 123;

    @setMetadata
    accessor b = 'b';

    @setMetadata
    fn() {}
}

const metadata = MyClass[Symbol.metadata]; // Haal metadata-informatie op

console.log(JSON.stringify(metadata)); // {"bar":true,"baz":true,"foo":true}
```

### Overerving

Overerving (inheritance) verwijst naar het mechanisme waarbij een klasse eigenschappen en methoden kan overerven van een andere klasse, bekend als de basisklasse of superklasse. De afgeleide klasse, ook wel de kindklasse of subklasse genoemd, kan de functionaliteit van de basisklasse uitbreiden en specialiseren door nieuwe eigenschappen en methoden toe te voegen of bestaande te overschrijven.

```typescript
class Animal {
    name: string;

    constructor(name: string) {
        this.name = name;
    }

    speak(): void {
        console.log('The animal makes a sound');
    }
}

class Dog extends Animal {
    breed: string;

    constructor(name: string, breed: string) {
        super(name);
        this.breed = breed;
    }

    speak(): void {
        console.log('Woof! Woof!');
    }
}

// Maak een instantie van de basisklasse
const animal = new Animal('Generic Animal');
animal.speak(); // The animal makes a sound

// Maak een instantie van de afgeleide klasse
const dog = new Dog('Max', 'Labrador');
dog.speak(); // Woof! Woof!"
```

TypeScript ondersteunt geen meervoudige overerving in de traditionele zin en staat in plaats daarvan overerving van een enkele basisklasse toe.
TypeScript ondersteunt wel meerdere interfaces. Een interface kan een contract definiëren voor de structuur van een object, en een klasse kan meerdere interfaces implementeren. Hierdoor kan een klasse gedrag en structuur van meerdere bronnen overerven.

```typescript
interface Flyable {
    fly(): void;
}

interface Swimmable {
    swim(): void;
}

class FlyingFish implements Flyable, Swimmable {
    fly() {
        console.log('Flying...');
    }

    swim() {
        console.log('Swimming...');
    }
}

const flyingFish = new FlyingFish();
flyingFish.fly();
flyingFish.swim();
```

Het trefwoord `class` in TypeScript is, net als in JavaScript, vaak aangeduid als syntactische suiker (syntactic sugar). Het werd geïntroduceerd in ECMAScript 2015 (ES6) om een vertrouwder syntaxis te bieden voor het maken van en werken met objecten op een klasse-gebaseerde manier. Het is echter belangrijk op te merken dat TypeScript, als een superset van JavaScript, uiteindelijk compileert naar JavaScript, dat in de kern op prototypes gebaseerd blijft.

### Statics

TypeScript heeft statische leden (static members). Om de statische leden van een klasse te benaderen, kun je de klassenaam gebruiken gevolgd door een punt, zonder dat je een object hoeft te maken.

```typescript
class OfficeWorker {
    static memberCount: number = 0;

    constructor(private name: string) {
        OfficeWorker.memberCount++;
    }
}

const w1 = new OfficeWorker('James');
const w2 = new OfficeWorker('Simon');
const total = OfficeWorker.memberCount;
console.log(total); // 2
```

### Eigenschapsinitialisatie

Er zijn verschillende manieren waarop je eigenschappen voor een klasse in TypeScript kunt initialiseren:

Inline:

In het volgende voorbeeld worden deze beginwaarden gebruikt wanneer een instantie van de klasse wordt gemaakt.

```typescript
class MyClass {
    property1: string = 'default value';
    property2: number = 42;
}
```

In de constructor:

```typescript
class MyClass {
    property1: string;
    property2: number;

    constructor() {
        this.property1 = 'default value';
        this.property2 = 42;
    }
}
```

Gebruik van constructorparameters:

```typescript
class MyClass {
    constructor(
        private property1: string = 'default value',
        public property2: number = 42
    ) {
        // Het is niet nodig om de waarden expliciet aan de eigenschappen toe te wijzen.
    }
    log() {
        console.log(this.property2);
    }
}
const x = new MyClass();
x.log();
```

### Method Overloading

Method overloading stelt een klasse in staat om meerdere methoden met dezelfde naam te hebben, maar met verschillende parametertypes of een ander aantal parameters. Hierdoor kunnen we een methode op verschillende manieren aanroepen op basis van de doorgegeven argumenten.

```typescript
class MyClass {
    add(a: number, b: number): number; // Overload signatuur 1
    add(a: string, b: string): string; // Overload signatuur 2

    add(a: number | string, b: number | string): number | string {
        if (typeof a === 'number' && typeof b === 'number') {
            return a + b;
        }
        if (typeof a === 'string' && typeof b === 'string') {
            return a.concat(b);
        }
        throw new Error('Invalid arguments');
    }
}

const r = new MyClass();
console.log(r.add(10, 5)); // Logt 15
```

## Generics

Generics stellen je in staat om herbruikbare componenten en functies te maken die met meerdere types kunnen werken. Met generics kun je types, functies en interfaces parametriseren, waardoor ze op verschillende types kunnen opereren zonder ze vooraf expliciet te specificeren.

Generics maken code flexibeler en herbruikbaar.

### Generiek Type

Om een generiek type te definiëren, gebruik je punthaakjes (`<>`) om de typeparameters te specificeren, bijvoorbeeld:

```typescript
function identity<T>(arg: T): T {
    return arg;
}
const a = identity('x');
const b = identity(123);

const getLen = <T,>(data: ReadonlyArray<T>) => data.length;
const len = getLen([1, 2, 3]);
```

### Generieke Classes

Generics kunnen ook op klassen worden toegepast; op deze manier kunnen ze met meerdere types werken door typeparameters te gebruiken. Dit is nuttig om herbruikbare klassedefinities te maken die op verschillende datatypes kunnen opereren met behoud van typeveiligheid.

```typescript
class Container<T> {
    private item: T;

    constructor(item: T) {
        this.item = item;
    }

    getItem(): T {
        return this.item;
    }
}

const numberContainer = new Container<number>(123);
console.log(numberContainer.getItem()); // 123

const stringContainer = new Container<string>('hello');
console.log(stringContainer.getItem()); // hello
```

### Generieke Constraints

Generieke parameters kunnen worden beperkt (constrained) met het trefwoord `extends`, gevolgd door een type of interface waaraan de typeparameter moet voldoen.

In het volgende voorbeeld moet T een eigenschap `length` bevatten om geldig te zijn:

<!-- skip -->
```typescript
const printLen = <T extends { length: number }>(value: T): void => {
    console.log(value.length);
};

printLen('Hello'); // 5
printLen([1, 2, 3]); // 3
printLen({ length: 10 }); // 10
printLen(123); // Ongeldig
```

Een interessante functie van generics, geïntroduceerd in versie 3.4 RC, is type-inference voor hogere-orde functies, die gepropageerde generieke type-argumenten introduceerde:

```typescript
declare function pipe<A extends any[], B, C>(
    ab: (...args: A) => B,
    bc: (b: B) => C
): (...args: A) => C;

declare function list<T>(a: T): T[];
declare function box<V>(x: V): { value: V };

const listBox = pipe(list, box); // <T>(a: T) => { value: T[] }
const boxList = pipe(box, list); // <V>(x: V) => { value: V }[]
```

Deze functionaliteit maakt typeveilige point-free programmeerstijl eenvoudiger, wat gebruikelijk is in functioneel programmeren.

### Generieke Contextuele Narrowing

Contextuele narrowing voor generics is het mechanisme in TypeScript waarmee de compiler het type van een generieke parameter kan vernauwen op basis van de context waarin deze wordt gebruikt; het is nuttig bij het werken met generieke types in voorwaardelijke statements:

```typescript
function process<T>(value: T): void {
    if (typeof value === 'string') {
        // Value is vernauwd tot type 'string'
        console.log(value.length);
    } else if (typeof value === 'number') {
        // Value is vernauwd tot type 'number'
        console.log(value.toFixed(2));
    }
}

process('hello'); // 5
process(3.14159); // 3.14
```

## Erased Structural Types

In TypeScript hoeven objecten niet overeen te komen met een specifiek, exact type. Als we bijvoorbeeld een object maken dat voldoet aan de eisen van een interface, kunnen we dat object gebruiken op plaatsen waar die interface vereist is, zelfs als er geen expliciete verbinding tussen hen was.
Voorbeeld:

```typescript
type NameProp1 = {
    prop1: string;
};

function log(x: NameProp1) {
    console.log(x.prop1);
}

const obj = {
    prop2: 123,
    prop1: 'Origin',
};

log(obj); // Geldig
```

## Namespacing

In TypeScript worden namespaces gebruikt om code te organiseren in logische containers, waardoor naamconflicten worden voorkomen en een manier wordt geboden om gerelateerde code te groeperen.
Het gebruik van het trefwoord `export` staat toegang tot de namespace toe in modules "buiten" de namespace.

```typescript
export namespace MyNamespace {
    export interface MyInterface1 {
        prop1: boolean;
    }
    export interface MyInterface2 {
        prop2: string;
    }
}

const a: MyNamespace.MyInterface1 = {
    prop1: true,
};
```

## Symbols

Symbols zijn een primitief datatype dat een onveranderlijke waarde vertegenwoordigt die gegarandeerd wereldwijd uniek is gedurende de levensduur van het programma.

Symbols kunnen worden gebruikt als keys voor objecteigenschappen en bieden een manier om niet-opsombare (non-enumerable) eigenschappen te maken.

```typescript
const key1: symbol = Symbol('key1');
const key2: symbol = Symbol('key2');

const obj = {
    [key1]: 'value 1',
    [key2]: 'value 2',
};

console.log(obj[key1]); // value 1
console.log(obj[key2]); // value 2
```

In WeakMaps en WeakSets zijn symbols nu toegestaan als keys.

## Triple-Slash Directives

Triple-slash directives zijn speciale opmerkingen die instructies geven aan de compiler over hoe een bestand moet worden verwerkt. Deze directives beginnen met drie opeenvolgende slashes (`///`) en worden doorgaans bovenaan een TypeScript-bestand geplaatst; ze hebben geen effect op het runtime-gedrag.

Triple-slash directives worden gebruikt om te verwijzen naar externe afhankelijkheden, het laadgedrag van modules te specificeren, bepaalde compilerfuncties in of uit te schakelen, en meer. Enkele voorbeelden:

Verwijzen naar een declaratiebestand:

<!-- skip -->
```typescript
/// <reference path="pad/naar/declaratie/bestand.d.ts" />
```

Het moduleformaat aangeven:

<!-- skip -->
```typescript
/// <amd|commonjs|system|umd|es6|es2015|none>
```

Compileropties inschakelen, in het volgende voorbeeld de strict-modus:

<!-- skip -->
```typescript
/// <strict|noImplicitAny|noUnusedLocals|noUnusedParameters>
```

## Type Manipulatie

### Types Maken van Types

Het is mogelijk om nieuwe types te maken door bestaande types samen te voegen, te manipuleren of te transformeren.

Intersection Types (`&`):

Stellen je in staat om meerdere types te combineren tot een enkel type:

```typescript
type A = { foo: number };
type B = { bar: string };
type C = A & B; // Intersection van A en B
const obj: C = { foo: 42, bar: 'hello' };
```

Union Types (`|`):

Stellen je in staat om een type te definiëren dat een van meerdere types kan zijn:

```typescript
type Result = string | number;
const value1: Result = 'hello';
const value2: Result = 42;
```

Mapped Types:

Stellen je in staat om de eigenschappen van een bestaand type te transformeren om een nieuw type te creëren:

```typescript
type Mutable<T> = {
    readonly [P in keyof T]: T[P];
};
type Person = {
    name: string;
    age: number;
};
type ImmutablePerson = Mutable<Person>; // Eigenschappen worden alleen-lezen
```

Conditional types:

Stellen je in staat om types te maken op basis van bepaalde voorwaarden:

```typescript
type ExtractParam<T> = T extends (param: infer P) => any ? P : never;
type MyFunction = (name: string) => number;
type ParamType = ExtractParam<MyFunction>; // string
```

### Indexed Access Types

In TypeScript is het mogelijk om de types van eigenschappen binnen een ander type te benaderen en te manipuleren met behulp van een index, `Type[Key]`.

```typescript
type Person = {
    name: string;
    age: number;
};

type AgeType = Person['age']; // number
```

```typescript
type MyTuple = [string, number, boolean];
type MyType = MyTuple[2]; // boolean
```

### Utility Types

Er kunnen verschillende ingebouwde utility types worden gebruikt om types te manipuleren; hieronder een lijst van de meest gebruikte:

#### Awaited<T>

Construeert een type dat recursief Promise-types uitpakt (unwraps).

```typescript
type A = Awaited<Promise<string>>; // string
```

#### Partial<T>

Construeert een type waarbij alle eigenschappen van T op optioneel zijn ingesteld.

```typescript
type Person = {
    name: string;
    age: number;
};

type A = Partial<Person>; // { name?: string | undefined; age?: number | undefined; }
```

#### Required<T>

Construeert een type waarbij alle eigenschappen van T op verplicht zijn ingesteld.

```typescript
type Person = {
    name?: string;
    age?: number;
};

type A = Required<Person>; // { name: string; age: number; }
```

#### Readonly<T>

Construeert een type waarbij alle eigenschappen van T op alleen-lezen (readonly) zijn ingesteld.

<!-- skip -->
```typescript
type Person = {
    name: string;
    age: number;
};

type A = Readonly<Person>;

const a: A = { name: 'Simon', age: 17 };
a.name = 'John'; // Ongeldig
```

#### Record<K, T>

Construeert een type met een set eigenschappen K van het type T.

```typescript
type Product = {
    name: string;
    price: number;
};

const products: Record<string, Product> = {
    apple: { name: 'Apple', price: 0.5 },
    banana: { name: 'Banana', price: 0.25 },
};

console.log(products.apple); // { name: 'Apple', price: 0.5 }
```

#### Pick<T, K>

Construeert een type door de gespecificeerde eigenschappen K uit T te kiezen.

```typescript
type Product = {
    name: string;
    price: number;
};

type Price = Pick<Product, 'price'>; // { price: number; }
```

#### Omit<T, K>

Construeert een type door de gespecificeerde eigenschappen K uit T weg te laten.

```typescript
type Product = {
    name: string;
    price: number;
};

type Name = Omit<Product, 'price'>; // { name: string; }
```

#### Exclude<T, U>

Construeert een type door alle waarden van het type U uit T uit te sluiten.

```typescript
type Union = 'a' | 'b' | 'c';
type MyType = Exclude<Union, 'a' | 'c'>; // b
```

#### Extract<T, U>

Construeert een type door alle waarden van het type U uit T te extraheren.

```typescript
type Union = 'a' | 'b' | 'c';
type MyType = Extract<Union, 'a' | 'c'>; // a | c
```

#### NonNullable<T>

Construeert een type door null en undefined uit T uit te sluiten.

```typescript
type Union = 'a' | null | undefined | 'b';
type MyType = NonNullable<Union>; // 'a' | 'b'
```

#### Parameters<T>

Extraheert de parametertypes van een functietype T.

```typescript
type Func = (a: string, b: number) => void;
type MyType = Parameters<Func>; // [a: string, b: number]
```

#### ConstructorParameters<T>

Extraheert de parametertypes van een constructorfunctietype T.

```typescript
class Person {
    constructor(
        public name: string,
        public age: number
    ) {}
}
type PersonConstructorParams = ConstructorParameters<typeof Person>; // [name: string, age: number]
const params: PersonConstructorParams = ['John', 30];
const person = new Person(...params);
console.log(person); // Person { name: 'John', age: 30 }
```

#### ReturnType<T>

Extraheert het return-type van een functietype T.

```typescript
type Func = (name: string) => number;
type MyType = ReturnType<Func>; // number
```

#### InstanceType<T>

Extraheert het instantietype van een klassetype T.

```typescript
class Person {
    name: string;

    constructor(name: string) {
        this.name = name;
    }

    sayHello() {
        console.log(`Hello, my name is ${this.name}!`);
    }
}

type PersonInstance = InstanceType<typeof Person>;

const person: PersonInstance = new Person('John');

person.sayHello(); // Hello, my name is John!
```

#### ThisParameterType<T>

Extraheert het type van de 'this'-parameter uit een functietype T.

```typescript
interface Person {
    name: string;
    greet(this: Person): void;
}
type PersonThisType = ThisParameterType<Person['greet']>; // Person
```

#### OmitThisParameter<T>

Verwijdert de 'this'-parameter uit een functietype T.

```typescript
function capitalize(this: String) {
    return this[0].toUpperCase + this.substring(1).toLowerCase();
}

type CapitalizeType = OmitThisParameter<typeof capitalize>; // () => string
```

#### ThisType<T>

Dient als markering voor een contextueel `this`-type.

<!-- skip -->
```typescript
type Logger = {
    log: (error: string) => void;
};

let helperFunctions: { [name: string]: Function } & ThisType<Logger> = {
    hello: function () {
        this.log('some error'); // Geldig omdat "log" deel uitmaakt van "this".
        this.update(); // Ongeldig
    },
};
```

#### Uppercase<T>

Zet de naam van het invoertype T om naar hoofdletters.

```typescript
type MyType = Uppercase<'abc'>; // "ABC"
```

#### Lowercase<T>

Zet de naam van het invoertype T om naar kleine letters.

```typescript
type MyType = Lowercase<'ABC'>; // "abc"
```

#### Capitalize<T>

Zet de eerste letter van de naam van het invoertype T om naar een hoofdletter.

```typescript
type MyType = Capitalize<'abc'>; // "Abc"
```

#### Uncapitalize<T>

Zet de eerste letter van de naam van het invoertype T om naar een kleine letter.

```typescript
type MyType = Uncapitalize<'Abc'>; // "abc"
```

#### NoInfer<T>

NoInfer is een utility type ontworpen om de automatische afleiding van types binnen de scope van een generieke functie te blokkeren.

Voorbeeld:

```typescript
// Automatische afleiding van types binnen de scope van een generieke functie.
function fn<T extends string>(x: T[], y: T) {
    return x.concat(y);
}
const r = fn(['a', 'b'], 'c'); // Type hier is ("a" | "b" | "c")[]
```

Met NoInfer:

<!-- skip -->
```typescript
// Voorbeeld functie die NoInfer gebruikt om type-inference te voorkomen
function fn2<T extends string>(x: T[], y: NoInfer<T>) {
    return x.concat(y);
}

const r2 = fn2(['a', 'b'], 'c'); // Fout: Type Argument van type '"c"' is niet toewijsbaar aan parameter van type '"a" | "b"'.
```

## Overige

### Fouten en Exception Handling

TypeScript stelt je in staat om fouten op te vangen en af te handelen met behulp van standaard JavaScript-mechanismen voor foutafhandeling:

Try-Catch-Finally blokken:

```typescript
try {
    // Code die mogelijk een fout gooit
} catch (error) {
    // Handal de fout af
} finally {
    // Code die altijd wordt uitgevoerd, finally is optioneel
}
```

Je kunt ook verschillende soorten fouten afhandelen:

```typescript
try {
    // Code die mogelijk verschillende soorten fouten gooit
} catch (error) {
    if (error instanceof TypeError) {
        // Handel TypeError af
    } else if (error instanceof RangeError) {
        // Handel RangeError af
    } else {
        // Handel andere fouten af
    }
}
```

Aangepaste Fouttypes:

Het is mogelijk om specifiekere fouten te specificeren door de `Error` klasse uit te breiden:

```typescript
class CustomError extends Error {
    constructor(message: string) {
        super(message);
        this.name = 'CustomError';
    }
}

throw new CustomError('Dit is een aangepaste fout.');
```

### Mixin Classes

Mixin classes stellen je in staat om gedrag van meerdere klassen te combineren en samen te stellen in een enkele klasse. Ze bieden een manier om functionaliteit te hergebruiken en uit te breiden zonder de noodzaak voor diepe overervingsketens.

```typescript
abstract class Identifiable {
    name: string = '';
    logId() {
        console.log('id:', this.name);
    }
}
abstract class Selectable {
    selected: boolean = false;
    select() {
        this.selected = true;
        console.log('Select');
    }
    deselect() {
        this.selected = false;
        console.log('Deselect');
    }
}
class MyClass {
    constructor() {}
}

// Breid MyClass uit met het gedrag van Identifiable en Selectable
interface MyClass extends Identifiable, Selectable {}

// Functie om mixins toe te passen op een klasse
function applyMixins(source: any, baseCtors: any[]) {
    baseCtors.forEach(baseCtor => {
        Object.getOwnPropertyNames(baseCtor.prototype).forEach(name => {
            let descriptor = Object.getOwnPropertyDescriptor(
                baseCtor.prototype,
                name
            );
            if (descriptor) {
                Object.defineProperty(source.prototype, name, descriptor);
            }
        });
    });
}

// Pas de mixins toe op MyClass
applyMixins(MyClass, [Identifiable, Selectable]);
let o = new MyClass();
o.name = 'abc';
o.logId();
o.select();
```

### Asynchrone Taalfuncties

Aangezien TypeScript een superset van JavaScript is, heeft het de ingebouwde asynchrone taalfuncties van JavaScript, zoals:

Promises:

Promises zijn een manier om asynchrone bewerkingen en hun resultaten af te handelen met methoden zoals `.then()` and `.catch()` om succes- en foutsituaties af te handelen.

Om meer te leren: [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

Async/await:

De trefwoorden async/await zijn een manier om een meer synchroon ogende syntaxis te bieden voor het werken met Promises. Het trefwoord `async` wordt gebruikt om een asynchrone functie te definiëren, en het trefwoord `await` wordt binnen een async-functie gebruikt om de uitvoering te pauzeren totdat een Promise is ingelost (resolved) of afgewezen (rejected).

Om meer te leren:
[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function)
[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/await](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/await)

De volgende API's worden goed ondersteund in TypeScript:

Fetch API:
[https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

Web Workers:
[https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API)

Shared Workers:
[https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker](https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker)

WebSocket:
[https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API)

### Iterators en Generators

Zowel iterators als generators worden goed ondersteund in TypeScript.

Iterators zijn objecten die het iterator-protocol implementeren en een manier bieden om elementen van een verzameling of reeks één voor één te benaderen. Het is een structuur die een verwijzing bevat naar het volgende element in de iteratie. Ze hebben een `next()` methode die de volgende waarde in de reeks retourneert, samen met een boolean die aangeeft of de reeks voltooid (`done`) is.

```typescript
class NumberIterator implements Iterable<number> {
    private current: number;

    constructor(
        private start: number,
        private end: number
    ) {
        this.current = start;
    }

    public next(): IteratorResult<number> {
        if (this.current <= this.end) {
            const value = this.current;
            this.current++;
            return { value, done: false };
        } else {
            return { value: undefined, done: true };
        }
    }

    [Symbol.iterator](): Iterator<number> {
        return this;
    }
}

const iterator = new NumberIterator(1, 3);

for (const num of iterator) {
    console.log(num);
}
```

Generators zijn speciale functies die zijn gedefinieerd met de `function*` syntaxis die het maken van iterators vereenvoudigt. Ze gebruiken het trefwoord `yield` om de reeks waarden te definiëren en pauzeren en hervatten automatisch de uitvoering wanneer waarden worden opgevraagd.

Generators maken het gemakkelijker om iterators te maken en zijn vooral nuttig voor het werken met grote of oneindige reeksen.

Voorbeeld:

```typescript
function* numberGenerator(start: number, end: number): Generator<number> {
    for (let i = start; i <= end; i++) {
        yield i;
    }
}

const generator = numberGenerator(1, 5);

for (const num of generator) {
    console.log(num);
}
```

TypeScript ondersteunt ook asynchrone iterators en asynchrone generators.

Om meer te leren:

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Generator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Generator)

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Iterator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Iterator)

### TsDocs JSDoc Referentie

Bij het werken met een JavaScript-codebase is het mogelijk om TypeScript te helpen het juiste type af te leiden door JSDoc-commentaar te gebruiken met aanvullende annotaties om type-informatie te verstrekken.

Voorbeeld:

```typescript
/**
 * Berekent de macht van een gegeven getal
 * @constructor
 * @param {number} base – De grondtalwaarde van de expressie
 * @param {number} exponent – De exponentwaarde van de expressie
 */
function power(base: number, exponent: number) {
    return Math.pow(base, exponent);
}
power(10, 2); // function power(base: number, exponent: number): number
```

De volledige documentatie is beschikbaar via deze link:
[https://www.typescriptlang.org/docs/handbook/jsdoc-supported-types.html](https://www.typescriptlang.org/docs/handbook/jsdoc-supported-types.html)

Vanaf versie 3.7 is het mogelijk om .d.ts typedefinities te genereren uit JavaScript JSDoc-syntaxis.
Meer informatie is hier te vinden:
[https://www.typescriptlang.org/docs/handbook/declaration-files/dts-from-js.html](https://www.typescriptlang.org/docs/handbook/declaration-files/dts-from-js.html)

### @types

Pakketten onder de @types organisatie zijn speciale pakketnaamconventies die worden gebruikt om typedefinities te leveren voor bestaande JavaScript-bibliotheken of modules. Bijvoorbeeld het gebruik van:

```shell
npm install --save-dev @types/lodash
```

Zal de typedefinities van `lodash` in je huidige project installeren.

Om bij te dragen aan de typedefinities van @types pakketten, kun je een pull request indienen bij [https://github.com/DefinitelyTyped/DefinitelyTyped](https://github.com/DefinitelyTyped/DefinitelyTyped).

### JSX

JSX (JavaScript XML) is een uitbreiding op de syntaxis van de taal JavaScript waarmee je HTML-achtige code binnen je JavaScript- of TypeScript-bestanden kunt schrijven. Het wordt veel gebruikt in React om de HTML-structuur te definiëren.

TypeScript breidt de mogelijkheden van JSX uit door typecontrole en statische analyse te bieden.

Om JSX te gebruiken, moet je de compileroptie `jsx` in je `tsconfig.json` bestand instellen. Twee veelvoorkomende configuratie-opties:

* "preserve": genereert .jsx bestanden waarbij de JSX ongewijzigd blijft. Deze optie vertelt TypeScript om de JSX-syntaxis onveranderd te laten en deze niet te transformeren tijdens het compilatieproces. Je kunt deze optie gebruiken als je een apart gereedschap hebt, zoals Babel, dat de transformatie afhandelt.
* "react": schakelt de ingebouwde JSX-transformatie van TypeScript in. React.createElement zal worden gebruikt.

Alle opties zijn hier beschikbaar:
[https://www.typescriptlang.org/tsconfig#jsx](https://www.typescriptlang.org/tsconfig#jsx)

### ES6 Modules

TypeScript ondersteunt ES6 (ECMAScript 2015) en vele daaropvolgende versies. Dit betekent dat je ES6-syntaxis kunt gebruiken, zoals arrow functions, template literals, klassen, modules, destructuring en meer.

Om ES6-functies in je project in te schakelen, kun je de eigenschap `target` specificeren in de tsconfig.json.

Een configuratievoorbeeld:

```json
{
  "compilerOptions": {
    "target": "es6",
    "module": "es6",
    "moduleResolution": "node",
    "sourceMap": true,
    "outDir": "dist"
  },
  "include": ["src"]
}
```

### ES7 Exponentiation Operator

De exponentiation (`**`) operator berekent de waarde die wordt verkregen door de eerste operand te verheffen tot de macht van de tweede operand. Het werkt vergelijkbaar met `Math.pow()`, maar met de toegevoegde mogelijkheid om BigInts als operanden te accepteren.
TypeScript ondersteunt deze operator volledig wanneer je als `target` in je tsconfig.json bestand `es2016` of een hogere versie gebruikt.

```typescript
console.log(2 ** (2 ** 2)); // 16
```

### Het for-await-of Statement

Dit is een JavaScript-functie die volledig wordt ondersteund in TypeScript en waarmee je over asynchrone itereerbare objecten kunt itereren vanaf targetversie es2018.

```typescript
async function* asyncNumbers(): AsyncIterableIterator<number> {
    yield Promise.resolve(1);
    yield Promise.resolve(2);
    yield Promise.resolve(3);
}

(async () => {
    for await (const num of asyncNumbers()) {
        console.log(num);
    }
})();
```

### Nieuwe target Meta-property

Je kunt in TypeScript de `new.target` meta-property gebruiken, waarmee je kunt bepalen of een functie of constructor is aangeroepen met de operator `new`. Het stelt je in staat om te detecteren of een object is gemaakt als resultaat van een constructor-aanroep.

```typescript
class Parent {
    constructor() {
        console.log(new.target); // Logt de constructorfunctie die is gebruikt om een instantie te maken
    }
}

class Child extends Parent {
    constructor() {
        super();
    }
}

const parentX = new Parent(); // [Function: Parent]
const child = new Child(); // [Function: Child]
```

### Dynamic Import Expressies

Het is mogelijk om modules conditioneel te laden of "lazy" te laden op aanvraag met behulp van het ECMAScript-voorstel voor dynamic import, dat wordt ondersteund in TypeScript.

De syntaxis voor dynamic import expressies in TypeScript is als volgt:

<!-- skip -->
```typescript
async function renderWidget() {
    const container = document.getElementById('widget');
    if (container !== null) {
        const widget = await import('./widget'); // Dynamische import
        widget.render(container);
    }
}

renderWidget();
```

### "tsc –watch"

Dit commando start de TypeScript-compiler met de parameter `–watch`, met de mogelijkheid om TypeScript-bestanden automatisch opnieuw te compileren wanneer ze worden gewijzigd.

```shell
tsc --watch
```

Vanaf TypeScript versie 4.9 vertrouwt bestandsbewaking voornamelijk op bestandssysteem-events, waarbij automatisch wordt teruggevallen op polling als een event-gebaseerde bewaker niet kan worden ingesteld.

### Non-null Assertion Operator

De Non-null Assertion Operator (Postfix !) ook wel Definite Assignment Assertions genoemd, is een TypeScript-functie waarmee je kunt beweren dat een variabele of eigenschap niet null of undefined is, zelfs als de statische type-analyse van TypeScript suggereert dat dit wel het geval zou kunnen zijn. Met deze functie is het mogelijk om elke expliciete controle te verwijderen.

```typescript
type Person = {
    name: string;
};

const printName = (person?: Person) => {
    console.log(`Naam is ${person!.name}`);
};
```

### Defaulted Declaraties

Defaulted declaraties worden gebruikt wanneer een variabele of parameter een standaardwaarde krijgt toegewezen. Dit betekent dat als er geen waarde wordt verstrekt voor die variabele of parameter, de standaardwaarde in plaats daarvan wordt gebruikt.

```typescript
function greet(name: string = 'Anoniem'): void {
    console.log(`Hallo, ${name}!`);
}
greet(); // Hallo, Anoniem!
greet('John'); // Hallo, John!
```

### Optional Chaining

De optional chaining operator `?.` werkt als de gewone puntoperator (`.`) voor het benaderen van eigenschappen of methoden. Het handelt echter op een gracieuze manier null of undefined waarden af door de expressie te beëindigen en `undefined` te retourneren, in plaats van een fout te gooien.

```typescript
type Person = {
    name: string;
    age?: number;
    address?: {
        street?: string;
        city?: string;
    };
};

const person: Person = {
    name: 'John',
};

console.log(person.address?.city); // undefined
```

### Nullish Coalescing Operator

De nullish coalescing operator `??` retourneert de rechterkant van de expressie als de linkerkant `null` of `undefined` is; anders retourneert hij de linkerkant.

```typescript
const foo = null ?? 'foo';
console.log(foo); // foo

const baz = 1 ?? 'baz';
const baz2 = 0 ?? 'baz';
console.log(baz); // 1
console.log(baz2); // 0
```

### Template Literal Types

Template Literal Types maken het mogelijk om stringwaarden op typeniveau te manipuleren en nieuwe stringtypes te genereren op basis van bestaande types. Ze zijn nuttig voor het maken van meer expressieve en preciezere types op basis van string-bewerkingen.

```typescript
type Department = 'engineering' | 'hr';
type Language = 'english' | 'spanish';
type Id = `${Department}-${Language}-id`; // "engineering-english-id" | "engineering-spanish-id" | "hr-english-id" | "hr-spanish-id"
```

### Functie Overloading

Functie-overloading stelt je in staat om meerdere functiesignaturen voor dezelfde functienaam te definiëren, elk met verschillende parametertypes en return-type.
Wanneer je een overloaded functie aanroept, gebruikt TypeScript de verstrekte argumenten om de juiste functiesignatuur te bepalen:

```typescript
function makeGreeting(name: string): string;
function makeGreeting(names: string[]): string[];

function makeGreeting(person: unknown): unknown {
    if (typeof person === 'string') {
        return `Hallo ${person}!`;
    } else if (Array.isArray(person)) {
        return person.map(name => `Hallo, ${name}!`);
    }
    throw new Error('Kan niet begroeten');
}

makeGreeting('Simon');
makeGreeting(['Simone', 'John']);
```

### Recursieve Types

Een Recursief Type is een type dat naar zichzelf kan verwijzen. Dit is nuttig voor het definiëren van datastructuren die een hiërarchische of recursieve structuur hebben (mogelijk oneindige nestbaarheid), zoals gelinkte lijsten, bomen en grafen.

```typescript
type ListNode<T> = {
    data: T;
    next: ListNode<T> | undefined;
};
```

### Recursieve Conditional Types

Het is mogelijk om complexe type-relaties te definiëren met behulp van logica en recursie in TypeScript.
Laten we het in eenvoudige termen uitleggen:

Conditional Types: stelt je in staat om types te definiëren op basis van boolean voorwaarden:

```typescript
type CheckNumber<T> = T extends number ? 'Getal' : 'Geen getal';
type A = CheckNumber<123>; // 'Getal'
type B = CheckNumber<'abc'>; // 'Geen getal'
```

Recursie: betekent een typedefinitie die naar zichzelf verwijst binnen zijn eigen definitie:

```typescript
type Json = string | number | boolean | null | Json[] | { [key: string]: Json };

const data: Json = {
    prop1: true,
    prop2: 'prop2',
    prop3: {
        prop4: [],
    },
};
```

Recursieve Conditional Types combineren zowel conditionele logica als recursie. Het betekent dat een typedefinitie van zichzelf afhankelijk kan zijn via conditionele logica, waardoor complexe en flexibele type-relaties ontstaan.

```typescript
type Flatten<T> = T extends Array<infer U> ? Flatten<U> : T;

type NestedArray = [1, [2, [3, 4], 5], 6];
type FlattenedArray = Flatten<NestedArray>; // 2 | 3 | 4 | 5 | 1 | 6
```

### ECMAScript Module Ondersteuning in Node

Node.js heeft ondersteuning voor ECMAScript-modules toegevoegd vanaf versie 15.3.0, en TypeScript heeft ECMAScript Module-ondersteuning voor Node.js sinds versie 4.7. Deze ondersteuning kan worden ingeschakeld door de eigenschap `module` met de waarde `nodenext` in het tsconfig.json bestand te gebruiken. Hier is een voorbeeld:

```json
{
  "compilerOptions": {
    "module": "nodenext",
    "outDir": "./lib",
    "declaration": true
  }
}
```

Node.js ondersteunt twee bestandsextensies voor modules: `.mjs` voor ES-modules en `.cjs` voor CommonJS-modules. De equivalente bestandsextensies in TypeScript zijn `.mts` voor ES-modules en `.cts` voor CommonJS-modules. Wanneer de TypeScript-compiler deze bestanden naar JavaScript transpileert, zal hij `.mjs` en `.cjs` bestanden maken.

Als je ES-modules in je project wilt gebruiken, kun je de eigenschap `type` op "module" instellen in je package.json bestand. Dit instrueert Node.js om het project te behandelen als een ES-module project.

Daarnaast ondersteunt TypeScript ook typedeclaraties in .d.ts bestanden. Deze declaratiebestanden bieden type-informatie voor bibliotheken of modules die in TypeScript zijn geschreven, waardoor andere ontwikkelaars deze kunnen gebruiken met TypeScript's typecontrole en automatische aanvulling.

### Assertion Functions

In TypeScript zijn assertion functions functies die de verificatie van een specifieke voorwaarde aangeven op basis van hun return-waarde. In hun eenvoudigste vorm onderzoekt een assert-functie een verstrekt predicaat en gooit een fout wanneer het predicaat als false wordt geëvalueerd.

```typescript
function isNumber(value: unknown): asserts value is number {
    if (typeof value !== 'number') {
        throw new Error('Geen getal');
    }
}
```

Of het kan worden gedeclareerd als functie-expressie:

```typescript
type AssertIsNumber = (value: unknown) => asserts value is number;
const isNumber: AssertIsNumber = value => {
    if (typeof value !== 'number') {
        throw new Error('Geen getal');
    }
};
```

Assertion functions vertonen overeenkomsten met type guards. Type guards werden oorspronkelijk geïntroduceerd om runtime-controles uit te voeren en het type van een waarde binnen een specifieke scope te garanderen.
Concreet is een type guard een functie die een type-predicaat evalueert en een boolean waarde retourneert die aangeeft of het predicaat true of false is. Dit verschilt enigszins van assertion functions, waarbij de intentie is om een fout te gooien in plaats van false te retourneren wanneer niet aan het predicaat wordt voldaan.

Voorbeeld van een type guard:

```typescript
const isNumber = (value: unknown): value is number => typeof value === 'number';
```

### Variadische Tuple Types

Variadische Tuple Types zijn functies die zijn geïntroduceerd in TypeScript versie 4.0. Laten we ze leren door te herhalen wat een tuple is:

Een tuple type is een array met een gedefinieerde lengte, waarbij het type van elk element bekend is:

```typescript
type Student = [string, number];
const [name, age]: Student = ['Simone', 20];
```

De term "variadisch" betekent een onbepaald aantal argumenten (accepts a variable number of arguments).

Een variadische tuple is een tuple type dat alle eigenschappen van voorheen heeft, maar waarvan de exacte vorm nog niet is gedefinieerd:

```typescript
type Bar<T extends unknown[]> = [boolean, ...T, number];

type A = Bar<[boolean]>; // [boolean, boolean, number]
type B = Bar<['a', 'b']>; // [boolean, 'a', 'b', number]
type C = Bar<[]>; // [boolean, number]
```

In de voorgaande code kunnen we zien dat de tuple-vorm wordt gedefinieerd door de doorgegeven `T` generic.

Variadische tuples kunnen meerdere generics accepteren, wat ze zeer flexibel maakt:

```typescript
type Bar<T extends unknown[], G extends unknown[]> = [...T, boolean, ...G];

type A = Bar<[number], [string]>; // [number, boolean, string]
type B = Bar<['a', 'b'], [boolean]>; // ["a", "b", boolean, boolean]
```

Met de nieuwe variadische tuples kunnen we:

* De spreads in de syntaxis van tuple types kunnen nu generiek zijn, zodat we hogere-orde bewerkingen op tuples en arrays kunnen vertegenwoordigen, zelfs wanneer we de werkelijke types waarop we opereren niet kennen.
* De rest-elementen kunnen overal in een tuple voorkomen.

Voorbeeld:

```typescript
type Items = readonly unknown[];

function concat<T extends Items, U extends Items>(
    arr1: T,
    arr2: U
): [...T, ...U] {
    return [...arr1, ...arr2];
}

concat([1, 2, 3], ['4', '5', '6']); // [1, 2, 3, "4", "5", "6"]
```

### Boxed Types

Boxed types verwijzen naar de wrapper-objecten die worden gebruikt om primitieve types als objecten te vertegenwoordigen. Deze wrapper-objecten bieden extra functionaliteit en methoden die niet direct beschikbaar zijn op de primitieve waarden.

Wanneer je een methode zoals `charAt` of `normalize` aanroept op een `string` primitief, verpakt JavaScript deze in een `String` object, roept de methode aan en gooit het object vervolgens weg.

Demonstratie:

```typescript
const originalNormalize = String.prototype.normalize;
String.prototype.normalize = function () {
    console.log(this, typeof this);
    return originalNormalize.call(this);
};
console.log('\u0041'.normalize());
```

TypeScript vertegenwoordigt dit onderscheid door afzonderlijke types te bieden voor de primitieven en hun overeenkomstige object-wrappers:

* string => String
* number => Number
* boolean => Boolean
* symbol => Symbol
* bigint => BigInt

De boxed types zijn doorgaans niet nodig. Vermijd het gebruik van boxed types en gebruik in plaats daarvan types voor de primitieven, bijvoorbeeld `string` in plaats van `String`.

### Covariantie en Contravariantie in TypeScript

Covariantie (Covariance) en Contravariantie (Contravariance) worden gebruikt om te beschrijven hoe relaties werken bij het omgaan met overerving of toewijzing van types.

Covariantie betekent dat een type-relatie de richting van overerving of toewijzing behoudt. Dus als een type A een subtype is van type B, dan wordt een array van type A ook beschouwd als een subtype van een array van type B. Het belangrijke om hier op te merken is dat de subtype-relatie behouden blijft; dit betekent dat covariantie subtypen accepteert maar geen supertypes.

Contravariantie betekent dat een type-relatie de richting van overerving of toewijzing omkeert. Dus als een type A een subtype is van type B, dan wordt een array van type B beschouwd als een subtype van een array van type A. De subtype-relatie wordt omgekeerd; dit betekent dat contravariantie supertypes accepteert maar geen subtypen.

Opmerkingen: Bivariantie betekent dat zowel supertypes als subtypen worden geaccepteerd.

Voorbeeld: Stel dat we een ruimte hebben voor alle dieren en een aparte ruimte voor alleen honden.

Bij covariantie kun je alle honden in de dierenruimte plaatsen omdat honden een soort dier zijn. Maar je kunt niet alle dieren in de hondenruimte plaatsen omdat er andere dieren tussen kunnen zitten.

Bij contravariantie kun je niet alle dieren in de hondenruimte plaatsen omdat de dierenruimte ook andere dieren kan bevatten. Je kunt echter wel alle honden in de dierenruimte plaatsen omdat alle honden ook dieren zijn.

<!-- skip -->
```typescript
// Covariantie voorbeeld
class Animal {
    name: string;
    constructor(name: string) {
        this.name = name;
    }
}

class Dog extends Animal {
    breed: string;
    constructor(name: string, breed: string) {
        super(name);
        this.breed = breed;
    }
}

let animals: Animal[] = [];
let dogs: Dog[] = [];

// Covariantie staat toe om een subtype (Dog) array toe te wijzen aan een supertype (Animal) array
animals = dogs;
dogs = animals; // Ongeldig: Type 'Animal[]' is niet toewijsbaar aan type 'Dog[]'

// Contravariantie voorbeeld
type Feed<in T> = (animal: T) => void;

let feedAnimal: Feed<Animal> = (animal: Animal) => {
    console.log(`Animal name: ${animal.name}`);
};

let feedDog: Feed<Dog> = (dog: Dog) => {
    console.log(`Dog name: ${dog.name}, Breed: ${dog.breed}`);
};

// Contravariantie staat toe om een supertype (Animal) callback toe te wijzen aan een subtype (Dog) callback
feedDog = feedAnimal;
feedAnimal = feedDog; // Ongeldig: Type 'Feed<Dog>' is niet toewijsbaar aan type 'Feed<Animal>'.
```

In TypeScript zijn type-relaties voor arrays covariant, terwijl type-relaties voor functieparameters contravariant zijn. Dit betekent dat TypeScript zowel covariantie als contravariantie vertoont, afhankelijk van de context.

#### Optionele Variantie-annotaties voor Type Parameters

Vanaf TypeScript 4.7.0 kunnen we de trefwoorden `out` en `in` gebruiken om specifiek te zijn over variantie-annotatie.

Gebruik voor covariantie het trefwoord `out`:

```typescript
type AnimalCallback<out T> = () => T; // T is hier covariant
```

En voor contravariantie het trefwoord `in`:

```typescript
type AnimalCallback<in T> = (value: T) => void; // T is hier contravariant
```

### Template String Pattern Index Signatures

Template string pattern index signatures stellen ons in staat om flexibele index-signatures te definiëren met behulp van template string-patronen. Deze functie stelt ons in staat om objecten te maken die kunnen worden geïndexeerd met specifieke patronen van string-keys, wat meer controle en specificiteit biedt bij het benaderen en manipuleren van eigenschappen.

TypeScript staat vanaf versie 4.4 index-signatures toe voor symbols en template string-patronen.

```typescript
const uniqueSymbol = Symbol('description');

type MyKeys = `key-${string}`;

type MyObject = {
    [uniqueSymbol]: string;
    [key: MyKeys]: number;
};

const obj: MyObject = {
    [uniqueSymbol]: 'Unique symbol key',
    'key-a': 123,
    'key-b': 456,
};

console.log(obj[uniqueSymbol]); // Unique symbol key
console.log(obj['key-a']); // 123
console.log(obj['key-b']); // 456
```

### De satisfies Operator

De operator `satisfies` stelt je in staat om te controleren of een gegeven type voldoet aan een specifieke interface of voorwaarde. Met andere woorden, het garandeert dat een type alle vereiste eigenschappen en methoden van een specifieke interface heeft. Het is een manier om ervoor te zorgen dat een variabele binnen een definitie van een type past.
Hier is een voorbeeld:

<!-- skip -->
```typescript
type Columns = 'name' | 'nickName' | 'attributes';

type User = Record<Columns, string | string[] | undefined>;

// Type-annotatie met gebruik van `User`
const user: User = {
    name: 'Simone',
    nickName: undefined,
    attributes: ['dev', 'admin'],
};

// In de volgende regels zal TypeScript niet in staat zijn om het type goed af te leiden
user.attributes?.map(console.log); // Property 'map' does not exist on type 'string | string[]'. Property 'map' does not exist on type 'string'.
user.nickName; // string | string[] | undefined

// Type-assertion met gebruik van `as`
const user2 = {
    name: 'Simon',
    nickName: undefined,
    attributes: ['dev', 'admin'],
} as User;

// Ook hier zal TypeScript niet in staat zijn om het type goed af te leiden
user2.attributes?.map(console.log); // Property 'map' does not exist on type 'string | string[]'. Property 'map' does not exist on type 'string'.
user2.nickName; // string | string[] | undefined

// Met de `satisfies` operator kunnen we de types nu wel goed afleiden
const user3 = {
    name: 'Simon',
    nickName: undefined,
    attributes: ['dev', 'admin'],
} satisfies User;

user3.attributes?.map(console.log); // TypeScript leidt correct af: string[]
user3.nickName; // TypeScript leidt correct af: undefined
```

### Type-Only Imports en Export

Type-Only Imports en Export stellen je in staat om types te importeren of exporteren zonder de waarden of functies die bij die types horen te importeren of exporteren. Dit kan nuttig zijn om de omvang van je bundel te verkleinen.

Om type-only imports te gebruiken, kun je het trefwoord `import type` gebruiken.

TypeScript staat het gebruik van zowel declaratie- als implementatie-bestandsextensies (.ts, .mts, .cts en .tsx) toe in type-only imports, ongeacht de instellingen van `allowImportingTsExtensions`.

Bijvoorbeeld:

<!-- skip -->
```typescript
import type { House } from './house.ts';
```

De volgende vormen worden ondersteund:

<!-- skip -->
```typescript
import type T from './mod';
import type { A, B } from './mod';
import type * as Types from './mod';
export type { T };
export type { T } from './mod';
```

### using Declaratie en Explicit Resource Management

Een `using` declaratie is een blok-gescoped, onveranderlijke binding, vergelijkbaar met `const`, gebruikt voor het beheren van wegwerpbare (disposable) bronnen. Bij initialisatie met een waarde wordt de methode `Symbol.dispose` van die waarde geregistreerd en vervolgens uitgevoerd bij het verlaten van de omsluitende blok-scope.

Dit is gebaseerd op ECMAScript's Resource Management functie, die nuttig is voor het uitvoeren van essentiële opschoontaken na het maken van een object, zoals het sluiten van verbindingen, het verwijderen van bestanden en het vrijgeven van geheugen.

Opmerkingen:

* Vanwege de recente introductie in TypeScript versie 5.2, ontbreekt in de meeste runtimes de native ondersteuning. Je hebt polyfills nodig voor: `Symbol.dispose`, `Symbol.asyncDispose`, `DisposableStack`, `AsyncDisposableStack`, `SuppressedError`.
* Bovendien moet je je tsconfig.json als volgt configureren:

```json
{
    "compilerOptions": {
        "target": "es2022",
        "lib": ["es2022", "esnext.disposable", "dom"]
    }
}
```

Voorbeeld:

<!-- skip -->
```typescript
//@ts-ignore
Symbol.dispose ??= Symbol('Symbol.dispose'); // Eenvoudige polyfill

const doWork = (): Disposable => {
    return {
        [Symbol.dispose]: () => {
            console.log('verwijderd (disposed)');
        },
    };
};

console.log(1);

{
    using work = doWork(); // Bron wordt gedeclareerd
    console.log(2);
} // Bron wordt opgeruimd (bijv., `work[Symbol.dispose]()` wordt uitgevoerd)

console.log(3);
```

De code zal loggen:

```shell
1
2
verwijderd (disposed)
3
```

Een bron die in aanmerking komt voor opruiming moet voldoen aan de `Disposable` interface:

```typescript
// lib.esnext.disposable.d.ts
interface Disposable {
    [Symbol.dispose](): void;
}
```

De `using` declaraties registreren bewerkingen voor het opruimen van bronnen in een stack, wat garandeert dat ze in omgekeerde volgorde van declaratie worden opgeruimd:

<!-- skip -->
```typescript
{
    using j = getA(),
        y = getB();
    using k = getC();
} // ruimt eerst `C` op, dan `B`, dan `A`.
```

Bronnen worden gegarandeerd opgeruimd, zelfs als er volgende code of uitzonderingen optreden. Dit kan ertoe leiden dat het opruimen zelf een uitzondering gooit, waardoor een andere mogelijk wordt onderdrukt. Om informatie over onderdrukte fouten te behouden, is een nieuwe native uitzondering, `SuppressedError`, geïntroduceerd.

#### await using Declaratie

Een `await using` declaratie verwerkt een asynchroon opruimbare bron. De waarde moet een `Symbol.asyncDispose` methode hebben, waarop wordt gewacht (awaited) aan het einde van het blok.

<!-- skip -->
```typescript
async function doWorkAsync() {
    await using work = doWorkAsync(); // Bron wordt gedeclareerd
} // Bron wordt opgeruimd (bijv., `await work[Symbol.asyncDispose]()` wordt uitgevoerd)
```

Voor een asynchroon opruimbare bron moet deze voldoen aan ofwel de `Disposable` of de `AsyncDisposable` interface:

```typescript
// lib.esnext.disposable.d.ts
interface AsyncDisposable {
    [Symbol.asyncDispose](): Promise<void>;
}
```

<!-- skip -->
```typescript
//@ts-ignore
Symbol.asyncDispose ??= Symbol('Symbol.asyncDispose'); // Eenvoudige polyfill

class DatabaseConnection implements AsyncDisposable {
    // Een methode die wordt aangeroepen wanneer het object asynchroon wordt opgeruimd
    [Symbol.asyncDispose]() {
        // Sluit de verbinding en retourneer een promise
        return this.close();
    }

    async close() {
        console.log('Verbinding wordt gesloten...');
        await new Promise(resolve => setTimeout(resolve, 1000));
        console.log('Verbinding gesloten.');
    }
}

async function doWork() {
    // Maak een nieuwe verbinding en ruim deze asynchroon op wanneer deze buiten de scope valt
    await using connection = new DatabaseConnection(); // Bron wordt gedeclareerd
    console.log('Wat werk aan het doen...');
} // Bron wordt opgeruimd (bijv., `await connection[Symbol.asyncDispose]()` wordt uitgevoerd)

doWork();
```

De code logt:

```shell
Wat werk aan het doen...
Verbinding wordt gesloten...
Verbinding gesloten.
```

De `using` and `await using` declaraties zijn toegestaan in de statements: `for`, `for-in`, `for-of`, `for-await-of`, `switch`.

### Import Attributes

Import Attributes van TypeScript 5.3 (labels voor imports) vertellen de runtime hoe om te gaan met modules (JSON, etc.). Dit verbetert de beveiliging door te zorgen voor duidelijke imports en sluit aan bij Content Security Policy (CSP) voor veiliger laden van bronnen. TypeScript garandeert dat ze geldig zijn, maar laat de interpretatie ervan aan de runtime over voor specifieke module-afhandeling.

Voorbeeld:

<!-- skip -->
```typescript
import config from './config.json' with { type: 'json' };
```

met dynamic import:

<!-- skip -->
```typescript
const config = import('./config.json', { with: { type: 'json' } });
```
