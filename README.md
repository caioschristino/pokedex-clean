# Description
DOJO Pokedex

# Requirements
-   MinSdk 24+ (Nougat 7.0)

## Languages, libraries and tools used
* [Kotlin](https://kotlinlang.org/)
* Android Support Libraries
* [Glide](https://github.com/bumptech/glide)
* [Retrofit](http://square.github.io/retrofit/)
* [OkHttp](http://square.github.io/okhttp/)
* [Gson](https://github.com/google/gson)
* [Mockito](http://site.mockito.org/)
* [Espresso](https://developer.android.com/training/testing/espresso/index.html)
* [Coroutines](https://kotlinlang.org/docs/reference/coroutines-overview.html)


Clean Architecture
-
![clean_architecture](https://user-images.githubusercontent.com/16631131/44717299-53711800-aac5-11e8-86b5-d3bda1035abc.png)

O projeto utiliza uma estratégia de interfaces para prover à inversão de dependência atráves da **Gateway Layer**, dispensando o uso de frameworks de Injeção de contexto.

Architectural approach
-
![clean_architecture_layers](https://user-images.githubusercontent.com/16631131/44717362-73084080-aac5-11e8-9029-10b3da073804.png)

**[Presentation Layer]** : Representada pela **Gateway Layer**, disponibilizando injeções de contexto(**Domain Layer**) à **ViewModel** assim como a implementação da mesma.

**[Domain Layer]** : Com Casos de Uso e interfaces de contrato.

**[Data Layer]** : Representada pela **Plugin Layer**, contém implementações concretas de contratos da **Domain Layer**, implementa regras de Guarda para Casos de Uso e definção de suporte à cache e api.


Android Architecture components with clean Architectural
-
![clean](https://user-images.githubusercontent.com/16631131/51852946-38d2f180-2338-11e9-918e-5bbcaaa4074f.png)