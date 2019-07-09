_This is a living document containing ChakraCore team's current priorities as well as release notes for previous releases. Future roadmap last updated 2/26/18._ 

All the changes done in the public repository flow into Chakra and Microsoft Edge on a regular basis as described in the [Contribution guidelines](https://github.com/Microsoft/ChakraCore/blob/master/CONTRIBUTING.md).

(Scroll to [Release Notes](#release-notes))

# Future

The following is a summary of the ChakraCore team's backlog for the next 6 months. Some completed items (either in a release or master branch) are included to provide the context and progress of the work.

## Language Innovation & Standards
* [x] Complete module implementation (ES6)
* [x] Complete Shared Memory and Atomics implementation
* [ ] Migrate JS Intl APIs to use ICU/CLDR on Windows
* [ ] ES2018+ features
  * [x] Implement promise.prototype.finally
  * [ ] Implement async generators & iterators
  * [ ] Implement object rest and spread
  * [ ] Implement new RegEx APIs
  * [ ] Implement new Intl APIs
* [ ] WebAssembly
  * [x] Enable WebAssembly MVP on by default
  * [ ] Enable post-MVP WebAssembly features

## Performance - Staying Fast and Lean
* [x] Optimize Object.assign/create
* [x] Optimize JSON.stringify/parse
* [x] Optimize ES6 for..of
  * [x] Enable inlining for try/catch/finally
* [ ] Improve performance for real-world sites
* [ ] Improve performance for ES2015+ features
* [ ] Reduce script parsing time
* [ ] Reduce GC fragmentation
* [ ] More type sharing

## Enhancing Host & Platform Support 
* **Node.js**
  * [x] Enable Node-ChakraCore on Mac and Linux.
  * [x] Support Chrome Debug Protocol in Node-ChakraCore.
  * [x] Enable Time Travel Debugging over Chrome Debug Protocol using VSCode
  * [x] Support N-API
  * [ ] Maintain [Node-ChakraCore](https://github.com/nodejs/node-chakracore) releases
  * [ ] Improve Node-ChakraCore performance based on benchmarks and real-world scenarios

* **Embedding**
  * [ ] Provide better debugging experience for ChakraCore embedders
    * [ ] Factor CrDP debugging shim in NodeChakraCore as a library to help enable debugging in applications embedding ChakraCore
  * [ ] Enable profiling

## Engineering Improvements
* [ ] Enable easier authoring of JavaScript built-ins in JavaScript.

# Release Notes

## ChakraCore 1.11

### [v1.11.11](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.11)
This patch release of ChakraCore 1.11 includes the following security fixes:

#### Security
- Changes to address CVE-2019-1001, CVE-2019-1062, CVE-2019-1092, CVE-2019-1103, CVE-2019-1106, CVE-2019-1107 [#6196](https://github.com/microsoft/ChakraCore/pull/6196)

### [v1.11.10](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.10)
This patch release of ChakraCore 1.11 includes the following security fixes:

#### Security
- Changes to address CVE-2019-0989 CVE-2019-0990, CVE-2019-0991, CVE-2019-0992, CVE-2019-0993, CVE-2019-1003, CVE-2019-1023, CVE-2019-1024, CVE-2019-1051, CVE-2019-1052 [#6155](https://github.com/microsoft/ChakraCore/pull/6155)

### [v1.11.9](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.9)
This patch release of ChakraCore 1.11 includes the following security fixes:

#### Security
- Changes to address CVE-2019-0911, CVE-2019-0912, CVE-2019-0913, CVE-2019-0914, CVE-2019-0915, CVE-2019-0916, CVE-2019-0917, CVE-2019-0922, CVE-2019-0923, CVE-2019-0924, CVE-2019-0925, CVE-2019-0927, CVE-2019-0933, CVE-2019-0937 [#6122](https://github.com/microsoft/ChakraCore/pull/6122)

### [v1.11.8](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.8)
This patch release of ChakraCore 1.11 includes the following security fixes:

#### Security
- Changes to address CVE-2019-0739, CVE-2019-0806, CVE-2019-0810, CVE-2019-0812, CVE-2019-0829, CVE-2019-0860, CVE-2019-0861 [#6087](https://github.com/Microsoft/ChakraCore/pull/6087)

### [v1.11.7](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.7)
This patch release of ChakraCore 1.11 includes the following security fixes:

#### Security
- Changes to address CVE-2019-0592, CVE-2019-0609, CVE-2019-0611, CVE-2019-0639, CVE-2019-0746, CVE-2019-0769, CVE-2019-0773, CVE-2019-0771 [#6016](https://github.com/Microsoft/ChakraCore/pull/6016)

### [v1.11.6](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.6)
This patch release of ChakraCore 1.11 includes the following security fixes:

#### Security
- Changes to address CVE-2019-0590, CVE-2019-0591, CVE-2019-0593, CVE-2019-0605, CVE-2019-0607, CVE-2019-0610, CVE-2019-0640, CVE-2019-0642, CVE-2019-0644, CVE-2019-0648, CVE-2019-0649, CVE-2019-0651, CVE-2019-0652, CVE-2019-0655, CVE-2019-0658 [#5936](https://github.com/Microsoft/ChakraCore/pull/5936) [#5940](https://github.com/Microsoft/ChakraCore/pull/5940)

### [v1.11.5](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.5)
This patch release of ChakraCore 1.11 includes security fixes, performance improvements, and bugfixes.

#### Security
- Changes to address CVE-2019-0539, CVE-2019-0567, CVE-2018-0568 [#5899](https://github.com/Microsoft/ChakraCore/pull/5899)

### [v1.11.4](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.4)
This patch release of ChakraCore 1.11 includes security fixes, performance improvements, and bugfixes.

#### Security
- Changes to address CVE-2018-8583, CVE-2018-8624, CVE-2018-8618, CVE-2018-8629, CVE-2018-8617 [#5869](https://github.com/Microsoft/ChakraCore/pull/5869)

### [v1.11.3](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.3)
This patch release of ChakraCore 1.11 includes security fixes, performance improvements, and bugfixes.

#### Security
- Changes to address CVE-2018-8541, CVE-2018-8542, CVE-2018-8543, CVE-2018-8551, CVE-2018-8555, CVE-2018-8556, CVE-2018-8557 and CVE-2018-8588 [#5827](https://github.com/Microsoft/ChakraCore/pull/5827)

### [v1.11.2](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.2)
This patch release of ChakraCore 1.11 includes security fixes, performance improvements, and bugfixes.

#### Security
- Changes to address CVE-2018-8473, CVE-2018-8500, CVE-2018-8503, CVE-2018-8505, CVE-2018-8510, CVE-2018-8511, and CVE-2018-8513 [#5764](https://github.com/Microsoft/ChakraCore/pull/5764)


### [v1.11.1](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.1)
This patch release of ChakraCore 1.11 includes security fixes, performance improvements, and bugfixes.

#### Security
- Changes to address CVE-2018-8315, CVE-2018-8354, CVE-2018-8367, CVE-2018-8452, CVE-2018-8456, CVE-2018-8459, CVE-2018-8465, CVE-2018-8466 and CVE-2018-8467 [#5688](https://github.com/Microsoft/ChakraCore/pull/5688)


### [v1.11.0](https://github.com/Microsoft/ChakraCore/releases/tag/v1.11.0)
ChakraCore 1.11.0 includes bug fixes, including a reliability fix relating to ETW tracing [#5632](https://github.com/Microsoft/ChakraCore/pull/5632)



## ChakraCore 1.10

### [v1.10.2](https://github.com/Microsoft/ChakraCore/releases/tag/v1.10.2)
This patch release of ChakraCore 1.10 includes security fixes, performance improvements, and bugfixes.

#### Security
- Changes to address CVE-2018-8380, CVE-2018-8359, CVE-2018-8385, CVE-2018-8390, CVE-2018-8266, CVE-2018-8384, CVE-2018-8372, CVE-2018-8355 and CVE-2018-8381 [#5596](https://github.com/Microsoft/ChakraCore/pull/5596)

### [v1.10.1](https://github.com/Microsoft/ChakraCore/releases/tag/v1.10.1)
This patch release of ChakraCore 1.10 includes security fixes, performance improvements, and bugfixes.

#### Security
- Changes to address CVE-2018-8275, CVE-2018-8276, CVE-2018-8279, CVE-2018-8280, CVE-2018-8283, CVE-2018-8286, CVE-2018-8287, CVE-2018-8288, CVE-2018-8290, CVE-2018-8291, CVE-2018-8294, CVE-2018-8298 [#5444](https://github.com/Microsoft/ChakraCore/pull/5444)


### [v1.10.0](https://github.com/Microsoft/ChakraCore/releases/tag/v1.10.0)

ChakraCore 1.10.0 includes more JavaScript and WebAssembly feature updates, performance enhancements, and JSRT APIs. See notable changes below.

Also shout-out to @rhuanjl, @fatcerberus, OSS-Fuzz, and Google Project Zero for their contributions during this release!

#### Language
- Improved support for Intl/ICU (see [use ICU on Windows](https://github.com/Microsoft/ChakraCore/wiki/Building-ChakraCore#windows--icu-experimental))
- Implement Intl.NumberFormat.prototype.formatToParts [#5105](https://github.com/Microsoft/ChakraCore/pull/5105)
- Implement Intl.PluralRules [#4940](https://github.com/Microsoft/ChakraCore/pull/4940)
- Implement Promise.prototype.finally [#3520](https://github.com/Microsoft/ChakraCore/pull/3520)
- Demote Dynamic Import support to behind a flag [f7bcf68cf](https://github.com/Microsoft/ChakraCore/commit/f7bcf68cfde698574581978a0984d1b1aba05a8b)

#### WebAssembly
- Enable sign extension operators on by default [#5136](https://github.com/Microsoft/ChakraCore/pull/5136)
- Implement non-trapping float to int conversions [#5129](https://github.com/Microsoft/ChakraCore/pull/5129) [#5014](https://github.com/Microsoft/ChakraCore/pull/5014)
- Implement atomic load/store [#4470](https://github.com/Microsoft/ChakraCore/pull/4470)
- Implement WebAssembly SIMD support behind experimental flag [#4200](https://github.com/Microsoft/ChakraCore/pull/4200)
- Implement WebAssembly Shared Memory (only available with SharedArrayBuffer on) [#4762](https://github.com/Microsoft/ChakraCore/pull/4762)

#### Performance
- Improved type-sharing for objects with getters/setters [#4283](https://github.com/Microsoft/ChakraCore/pull/4283) and for function objects [#4748](https://github.com/Microsoft/ChakraCore/pull/4748) [#4818](https://github.com/Microsoft/ChakraCore/pull/4818)
- Enable inlining for callback functions [#5081](https://github.com/Microsoft/ChakraCore/pull/5081)
- Improved performance for Array.prototype.filter [#5137](https://github.com/Microsoft/ChakraCore/pull/5137), Object.assign [#4852](https://github.com/Microsoft/ChakraCore/pull/4852) [#4817](https://github.com/Microsoft/ChakraCore/pull/4817), Map/Set [#4816](https://github.com/Microsoft/ChakraCore/pull/4816), and JSON.Stringify [#4907](https://github.com/Microsoft/ChakraCore/pull/4907) [#4831](https://github.com/Microsoft/ChakraCore/pull/4831)
- Improved optimizations for property access in loops [#5110](https://github.com/Microsoft/ChakraCore/pull/5110)
- Optimizations to minimize performance impact from Spectre mitigations 

#### JSRT
- Add JsGetPromiseState and JsGetPromiseResult [#5138](https://github.com/Microsoft/ChakraCore/pull/5138) [#5131](https://github.com/Microsoft/ChakraCore/pull/5131)
- Add JsGetProxyProperties [#4806](https://github.com/Microsoft/ChakraCore/pull/4806)
- Add JsRuntimeAttributeDisableExecutablePageAllocation attribute [#4797](https://github.com/Microsoft/ChakraCore/pull/4797)
- Add JsGetModuleNamespace [#4707](https://github.com/Microsoft/ChakraCore/pull/4707)
- Add JsSetHostPromiseRejectionTracker to process unhandled promise rejections [#4608](https://github.com/Microsoft/ChakraCore/pull/4608)
- Add JsCreateEnhancedFunction for native callbacks with `new.target` [#4529](https://github.com/Microsoft/ChakraCore/pull/4529)
- Add JsCreateExternalObjectWithPrototype [#4267](https://github.com/Microsoft/ChakraCore/pull/4267)
- Add Symbol support in JsObject[Has/Get/Set/....] APIs [#4209](https://github.com/Microsoft/ChakraCore/pull/4209)

#### Diagnostics
- Enable support for ETW events on xplat via LTTng [#4314](https://github.com/Microsoft/ChakraCore/pull/4314)


## ChakraCore 1.8

### [v1.8.5](https://github.com/Microsoft/ChakraCore/releases/tag/v1.8.5)
This patch release of ChakraCore 1.8 includes security fixes, performance improvements, and bugfixes.

#### Security
- Changes to address CVE-2018-8227, CVE-2018-8229 and CVE-2018-8236 [#5298](https://github.com/Microsoft/ChakraCore/pull/5298)


### [v1.8.4](https://github.com/Microsoft/ChakraCore/releases/tag/v1.8.4)
This patch release of ChakraCore 1.8 includes security fixes, performance improvements, and bugfixes.

#### Security
- Changes to address CVE-2018-0954, CVE-2018-1022, CVE-2018-8133, CVE-2018-0943, CVE-2018-0953, CVE-2018-8130, CVE-2018-0946, CVE-2018-8177, CVE-2018-8128, CVE-2018-8178, CVE-2018-8137, CVE-2018-8139, CVE-2018-0945 and Spectre [#5116](https://github.com/Microsoft/ChakraCore/pull/5116)

### [v1.8.3](https://github.com/Microsoft/ChakraCore/releases/tag/v1.8.3)
This patch release of ChakraCore 1.8 includes security fixes, performance improvements, and bugfixes.

#### Security
- Change to address CVE-2018-0980, CVE-2018-1019, CVE-2018-0995, CVE-2018-0993, CVE-2018-0979, CVE-2018-0990 and CVE-2018-0994 [#4963](https://github.com/Microsoft/ChakraCore/pull/4963)


### [v1.8.2](https://github.com/Microsoft/ChakraCore/releases/tag/v1.8.2)
This patch release of ChakraCore 1.8 includes security fixes, performance improvements, and bugfixes.

#### Security
- Change to address CVE-2018-0930, CVE-2018-0891, CVE-2018-0873, CVE-2018-0874, CVE-2018-0937, CVE-2018-0872, CVE-2018-0936, CVE-2018-0939, CVE-2018-0876, CVE-2018-0931, CVE-2018-0934, CVE-2018-0933, and an ACG bypass [#4812](https://github.com/Microsoft/ChakraCore/pull/4812)

### [v1.8.1](https://github.com/Microsoft/ChakraCore/releases/tag/v1.8.1)
This patch release of ChakraCore 1.8 includes security fixes, performance improvements, and bugfixes.

#### Security
- Change to address CVE-2018-0857, CVE-2018-0860, CVE-2018-0859, CVE-2018-0840, CVE-2018-0834, CVE-2018-0837, CVE-2018-0838, CVE-2018-0856, CVE-2018-0836, CVE-2018-0835, CVE-2018-0866, CVE-2018-0858, and Spectre [#4676](https://github.com/Microsoft/ChakraCore/pull/4676)

### [v1.8.0](https://github.com/Microsoft/ChakraCore/releases/tag/v1.8.0)

ChakraCore 1.8.0 includes more JavaScript and WebAssembly feature updates and performance enhancements. See notable changes below.

- [#3855](https://github.com/Microsoft/ChakraCore/pull/3855) Removed support for building with VS2013
- Several improvements to regex performance
- Performance improvements to `Object.assign`, `Object.create` and `Object.hasOwnProperty`
- Adding support for Arm64
- [#3553](https://github.com/Microsoft/ChakraCore/pull/3553) Experimental: Introduce "lite" ChakraCore build
- [#3594](https://github.com/Microsoft/ChakraCore/pull/3594) Byte code size and serialized byte code size optimizations (15-20% serialized byte code size reduction)
- [#3681](https://github.com/Microsoft/ChakraCore/pull/3681) add inlining support for asm.js/wasm
- [#3832](https://github.com/Microsoft/ChakraCore/pull/3832) Enable inlining into functions which have try-catch/try-finally
- [#3846](https://github.com/Microsoft/ChakraCore/pull/3846) Add support for a Recycler-managed "Host Heap" to facilitate tracing of objects which relate to scriptable types
- [#3931](https://github.com/Microsoft/ChakraCore/pull/3931) Add JSRT API `JsLessThan`
- [#4077](https://github.com/Microsoft/ChakraCore/pull/4077) Optimized `JSON.stringify` and `JSON.parse`
- [#4118](https://github.com/Microsoft/ChakraCore/pull/4118) Share types (i.e., allow PathTypeHandlers) for properties with non-standard attributes (non-writable, etc.).
- [#3875](https://github.com/Microsoft/ChakraCore/pull/3875) jsrt: added JsObject Delete/Get/Has/OwnP../Set Property methods
- [#4531](https://github.com/Microsoft/ChakraCore/pull/4531) Fix and enable wasm on xplat

## ChakraCore 1.7

### [v1.7.6](https://github.com/Microsoft/ChakraCore/releases/tag/v1.7.6)
This patch release of ChakraCore 1.7 includes security fixes, performance improvements, and bugfixes.

#### Security
- Change to address CVE-2018-0758, CVE-2018-0762, CVE-2018-0767, CVE-2018-0768, CVE-2018-0769, CVE-2018-0770, CVE-2018-0772, CVE-2018-0773, CVE-2018-0774, CVE-2018-0775, CVE-2018-0776, CVE-2018-0777, CVE-2018-0778, CVE-2018-0780, CVE-2018-0781 [#4503](https://github.com/Microsoft/ChakraCore/pull/4503)

### [v1.7.5](https://github.com/Microsoft/ChakraCore/releases/tag/v1.7.5)
This patch release of ChakraCore 1.7 includes security fixes, performance improvements, and bugfixes.

#### Security
- Change to address CVE-2017-11889, CVE-2017-11893, CVE-2017-11894, CVE-2017-11905, CVE-2017-11908, CVE-2017-11909, CVE-2017-11910, CVE-2017-11911, CVE-2017-11912, CVE-2017-11914, CVE-2017-11916, CVE-2017-11918, CVE-2017-11919, CVE-2017-11930 [#4411](https://github.com/Microsoft/ChakraCore/pull/4411)

### [v1.7.4](https://github.com/Microsoft/ChakraCore/releases/tag/v1.7.4)
This patch release of ChakraCore 1.7 includes security fixes, performance improvements, and bugfixes.

#### Security
- Change to address CVE-2017-11791, CVE-2017-11836, CVE-2017-11837, CVE-2017-11838, CVE-2017-11840, CVE-2017-11841, CVE-2017-11843, CVE-2017-11846, CVE-2017-11858, CVE-2017-11861, CVE-2017-11862, CVE-2017-11870, CVE-2017-11871, CVE-2017-11873, CVE-2017-11874, CVE-2017-11866, CVE-2017-11859 [#4226](https://github.com/Microsoft/ChakraCore/pull/4226)

### [v1.7.3](https://github.com/Microsoft/ChakraCore/releases/tag/v1.7.3)
This patch release of ChakraCore 1.7 includes security fixes, performance improvements, and bugfixes.

#### Security
- Change to address CVE-2017-11792, CVE-2017-11796, CVE-2017-11797, CVE-2017-11799, CVE-2017-11801, CVE-2017-11802, CVE-2017-11805, CVE-2017-11806, CVE-2017-11807, CVE-2017-11808, CVE-2017-11809, CVE-2017-11811, CVE-2017-11812, CVE-2017-11821 [#3917](https://github.com/Microsoft/ChakraCore/pull/3917)

### [v1.7.2](https://github.com/Microsoft/ChakraCore/releases/tag/v1.7.2)

This patch release of ChakraCore 1.7 includes security fixes, performance improvements, and bugfixes.

#### Security
- Change to address CVE-2017-8741, CVE-2017-8748, CVE-2017-11767, CVE-2017-8756, CVE-2017-8753, CVE-2017-8729, CVE-2017-8739, CVE-2017-8751, CVE-2017-8757, CVE-2017-11764, CVE-2017-8660, CVE-2017-8755, CVE-2017-8649, CVE-2017-8740, CVE-2017-8752 [#3729](https://github.com/Microsoft/ChakraCore/pull/3729)

### [v1.7.1](https://github.com/Microsoft/ChakraCore/releases/tag/v1.7.1)

This patch release of ChakraCore 1.7 includes security fixes, performance improvements and JSRT API changes. See notable changes below.

#### Security
- Change to address CVE-2017-0228, CVE-2017-8634, CVE-2017-8635, CVE-2017-8636, CVE-2017-8637, CVE-2017-8638, CVE-2017-8640, CVE-2017-8641, CVE-2017-8645, CVE-2017-8646, CVE-2017-8647, CVE-2017-8655, CVE-2017-8656, CVE-2017-8657, CVE-2017-8658, CVE-2017-8659, CVE-2017-8670, CVE-2017-8671, CVE-2017-8672, CVE-2017-8674 [#3509](https://github.com/Microsoft/ChakraCore/pull/3509)

#### Performance
- Remove tzdata sync calls on xplat [#3420](https://github.com/Microsoft/ChakraCore/pull/3420)

#### JSRT
- Add [JsGetDataViewInfo](https://github.com/Microsoft/ChakraCore/wiki/JsGetDataViewInfo) [#3462](https://github.com/Microsoft/ChakraCore/pull/3462)
- Modify [JsCopyString](https://github.com/Microsoft/ChakraCore/wiki/JsCopyString) to return actual count of utf8 bytes [#3433](https://github.com/Microsoft/ChakraCore/pull/3433)


### [v1.7.0](https://github.com/Microsoft/ChakraCore/releases/tag/v1.7.0)

ChakraCore 1.7.0 includes performance improvements and support for building Node-ChakraCore with link-time optimizations. It adds the following new JSRT APIs:

- [JsHasOwnProperty](https://github.com/Microsoft/ChakraCore/wiki/JsHasOwnProperty) [#3316](https://github.com/Microsoft/ChakraCore/pull/3316).
- [JsCopyStringOneByte](https://github.com/Microsoft/ChakraCore/wiki/JsCopyStringOneByte) [#3408](https://github.com/Microsoft/ChakraCore/pull/3408).

## ChakraCore 1.6

### [v1.6.2](https://github.com/Microsoft/ChakraCore/releases/tag/v1.6.2)

This patch release of ChakraCore 1.6 includes the following security fixes:

#### Security
- Change to address CVE-2017-8741, CVE-2017-8748, CVE-2017-11767, CVE-2017-8756, CVE-2017-8753, CVE-2017-8729, CVE-2017-8739, CVE-2017-8751, CVE-2017-8757, CVE-2017-11764, CVE-2017-8660, CVE-2017-8755, CVE-2017-8649, CVE-2017-8740, CVE-2017-8752 [#3729](https://github.com/Microsoft/ChakraCore/pull/3729)

### [v1.6.1](https://github.com/Microsoft/ChakraCore/releases/tag/v1.6.1)

This patch release of ChakraCore 1.6 includes security fixes and bug fixes. See notable changes below.

#### Security
- Change to address CVE-2017-0228, CVE-2017-8634, CVE-2017-8635, CVE-2017-8636, CVE-2017-8637, CVE-2017-8638, CVE-2017-8640, CVE-2017-8641, CVE-2017-8645, CVE-2017-8646, CVE-2017-8647, CVE-2017-8655, CVE-2017-8656, CVE-2017-8657, CVE-2017-8658, CVE-2017-8659, CVE-2017-8670, CVE-2017-8671, CVE-2017-8672, CVE-2017-8674 [#3509](https://github.com/Microsoft/ChakraCore/pull/3509)

### [v1.6.0](https://github.com/Microsoft/ChakraCore/releases/tag/v1.6.0)

ChakraCore 1.6.0 includes more JavaScript and WebAssembly feature updates and performance enhancements. See notable changes below.

#### Language
- Enable WebAssembly MVP on by default [#2447](https://github.com/Microsoft/ChakraCore/pull/2447)
- Enable SharedArrayBuffer on by default [#2939](https://github.com/Microsoft/ChakraCore/pull/2939)
- Enable [dynamic module import](https://github.com/tc39/proposal-dynamic-import) [#2913](https://github.com/Microsoft/ChakraCore/pull/2913)
- Support ES6 iterators for DOM objects [58ac5aeb7](https://github.com/Microsoft/ChakraCore/commit/58ac5aeb79063bec71aef310e46863001d926410)
- Remove SIMD support in JavaScript [#3296](https://github.com/Microsoft/ChakraCore/pull/3296)

#### Performance
- Support function body (re-)deferral in lexical scopes and parameter scopes [#2666](https://github.com/Microsoft/ChakraCore/pull/2666)
- Use PolymorphicInlineCache for obj[string] pattern [#2883](https://github.com/Microsoft/ChakraCore/pull/2883)
- Enable optimizer on functions with try/finally [#2954](https://github.com/Microsoft/ChakraCore/pull/2954)

## ChakraCore 1.5

### [v1.5.3](https://github.com/Microsoft/ChakraCore/releases/tag/v1.5.3)

This patch release of ChakraCore 1.5 includes the following security fixes:

- Change to address CVE-2017-8598, CVE-2017-8601, CVE-2017-8603, CVE-2017-8604, CVE-2017-8606, CVE-2017-8607, CVE-2017-8608, CVE-2017-8609, CVE-2017-8610, CVE-2017-8619 [#3341](https://github.com/Microsoft/ChakraCore/pull/3341)

### [v1.5.2](https://github.com/Microsoft/ChakraCore/releases/tag/v1.5.2)

This patch release of ChakraCore 1.5 includes the following security fixes:

- Change to address CVE-2017-0228, CVE-2017-8499, CVE-2017-8518, CVE-2017-8520, CVE-2017-8522, CVE-2017-8524, CVE-2017-8548 [#3166](https://github.com/Microsoft/ChakraCore/pull/3166)

### [v1.5.1](https://github.com/Microsoft/ChakraCore/releases/tag/v1.5.1)

This patch release of ChakraCore 1.5 includes a fix for a handle leak when creating multiple runtimes [#3092](https://github.com/Microsoft/ChakraCore/pull/3092)

### [v1.5.0](https://github.com/Microsoft/ChakraCore/releases/tag/v1.5.0)

ChakraCore 1.5.0 includes cross-platform concurrent/partial GC support and a set of new JSRT APIs among other changes. See notable changes below.

- Enable broader software-based write barrier support in ChakraCore GC [#2372](https://github.com/Microsoft/ChakraCore/pull/2372)
- Turn on ChakraCore concurrent/partial GC for Linux/OSX
- New experimental JSRT APIs
    * [JsCreatePromise](https://github.com/Microsoft/ChakraCore/wiki/JsCreatePromise) - add API to create promise [#2594](https://github.com/Microsoft/ChakraCore/pull/2594)
    * [JsGetAndClearExceptionWithMetadata](https://github.com/Microsoft/ChakraCore/wiki/JsGetAndClearExceptionWithMetadata) - add API to clear exception and expose additional information [#2936](https://github.com/Microsoft/ChakraCore/pull/2936)
    * [JsWeakRef](https://github.com/Microsoft/ChakraCore/wiki/JsWeakRef)/[JsCreateWeakReference](https://github.com/Microsoft/ChakraCore/wiki/JsCreateWeakReference)/[JsGetWeakReferenceValue](https://github.com/Microsoft/ChakraCore/wiki/JsGetWeakReferenceValue) - add weak reference APIs [#2948](https://github.com/Microsoft/ChakraCore/pull/2948)

## ChakraCore 1.4

### [v1.4.5](https://github.com/Microsoft/ChakraCore/releases/tag/v1.4.5)

This patch release of ChakraCore 1.4 includes a fix for a handle leak when creating multiple runtimes [#3092](https://github.com/Microsoft/ChakraCore/pull/3092).

### [v1.4.4](https://github.com/Microsoft/ChakraCore/releases/tag/v1.4.4)

This patch release of ChakraCore 1.4 includes the following security fixes:

- Change to address CVE-2017-0229, CVE-2017-0223, CVE-2017-0224, CVE-2017-0252, CVE-2017-0230, CVE-2017-0234, CVE-2017-0235, CVE-2017-0236, CVE-2017-0228, CVE-2017-0238, CVE-2017-0266
[#2959](https://github.com/Microsoft/ChakraCore/pull/2959)

### [v1.4.3](https://github.com/Microsoft/ChakraCore/releases/tag/v1.4.3)
 
This patch release of ChakraCore 1.4 includes the following fixes:
- Change to address CVE-2017-0093 and CVE-2017-0208 [#2834](https://github.com/Microsoft/ChakraCore/pull/2834)
- Internal fixes in Windows 10 Creators Update [#2826](https://github.com/Microsoft/ChakraCore/pull/2826)

### [v1.4.2](https://github.com/Microsoft/ChakraCore/releases/tag/v1.4.2)

This patch release of ChakraCore 1.4 includes the following security fixes:
- Change to address CVE-2017-0067, CVE-2017-0150, CVE-2017-0138, CVE-2017-0094, CVE-2017-0132, CVE-2017-0133, CVE-2017-0134, CVE-2017-0137, CVE-2017-0071, CVE-2017-0151, CVE-2017-0141, CVE-2017-0196, CVE-2017-0136, CVE-2017-0152, CVE-2017-0010, CVE-2017-0035, CVE-2017-0015, CVE-2017-0028
[#2697](https://github.com/Microsoft/ChakraCore/pull/2697)

### [v1.4.1](https://github.com/Microsoft/ChakraCore/releases/tag/v1.4.1)

This patch release of ChakraCore 1.4 enables using ChakraCore [NuGet packages](https://github.com/Microsoft/ChakraCore/wiki/NuGet-Packages) for developing .NET and native applications ([#2266](https://github.com/Microsoft/ChakraCore/pull/2266), [#85](https://github.com/Microsoft/ChakraCore/issues/85)) and includes other bug fixes.

### [v1.4.0](https://github.com/Microsoft/ChakraCore/releases/tag/v1.4.0)

ChakraCore 1.4.0 includes cross-platform JIT support and experimental WebAssembly support along with other language, performance and JSRT updates. See notable changes below.
 
- ChakraCore JIT on Linux and MacOS [#1591](https://github.com/Microsoft/ChakraCore/pull/1591) [#1744](https://github.com/Microsoft/ChakraCore/pull/1744)
- Enhance [Time Travel Debugging](https://github.com/nodejs/node-chakracore/blob/59950ad1e86fee5b872d203adc1929795ff63428/TTD-README.md) support
- Enable [Async Functions](https://tc39.github.io/ecmascript-asyncawait/#async-function-definitions) by default [#1691](https://github.com/Microsoft/ChakraCore/pull/1691)
- Enable [SharedArrayBuffer](https://github.com/tc39/ecmascript_sharedmem) under experimental flag [#1759](https://github.com/Microsoft/ChakraCore/pull/1759)
- Enable WebAssembly [browser preview](http://webassembly.org/roadmap/) support under experimental flag [#1985](https://github.com/Microsoft/ChakraCore/pull/1985)
- Update JSRT String APIs (experimental) [#1830](https://github.com/Microsoft/ChakraCore/pull/1830) 
- Memory reduction through function body redeferral [#1585](https://github.com/Microsoft/ChakraCore/pull/1585)
- Add out-of-process JIT support in Microsoft Edge [#1561](https://github.com/Microsoft/ChakraCore/pull/1561)

## ChakraCore 1.3

### [v1.3.2](https://github.com/Microsoft/ChakraCore/releases/tag/v1.3.2)

This patch release of ChakraCore 1.3 includes the following security fixes:

- Change to address bad binding of async arrow function parameters [#2219](https://github.com/Microsoft/ChakraCore/pull/2219)
- All fixes included in [v1.2.3](#v123)

### [v1.3.1](https://github.com/Microsoft/ChakraCore/releases/tag/v1.3.1)

This patch release of ChakraCore 1.3 includes the following security fixes:

- Change to address CVE-2016-7207 [#1979](https://github.com/Microsoft/ChakraCore/pull/1979)
- All fixes included in [v1.2.2](#v122)

### [v1.3.0](https://github.com/Microsoft/ChakraCore/releases/tag/v1.3.0)

Release 1.3.0 includes experimental support on x64 Linux/OSX, experimental JSRT debugging APIs,
and other language and performance updates. See notable changes below.

#### Cross-platform
- ChakraCore interpreter and runtime on x64 Linux (still working on JIT or concurrent/partial GC)
- ChakraCore interpreter and runtime on x64 OSX (still working on  JIT or concurrent/partial GC)
[#1134](https://github.com/Microsoft/ChakraCore/pull/1134)

#### Language
- Enable [Symbol.toStringTag](http://www.ecma-international.org/ecma-262/6.0/#sec-symbol.tostringtag)
by default [#1383](https://github.com/Microsoft/ChakraCore/pull/1383)
- Enable [String.prototype.padStart](https://tc39.github.io/ecma262/#sec-string.prototype.padstart)
and [String.prototype.padEnd](https://tc39.github.io/ecma262/#sec-string.prototype.padend)
by default [#1257](https://github.com/Microsoft/ChakraCore/pull/1257)
- Enable [Symbol.prototype[@@toPrimitive]](http://www.ecma-international.org/ecma-262/6.0/#sec-symbol.prototype-@@toprimitive) and [Date.prototype[@@toPrimitive]](http://www.ecma-international.org/ecma-262/6.0/#sec-date.prototype-@@toprimitive)
under experimental flag [#1319](https://github.com/Microsoft/ChakraCore/pull/1319)
- Enable [Symbol.isConcatSpreadable](http://www.ecma-international.org/ecma-262/6.0/#sec-symbol.isconcatspreadable)
under experimental flag [#1198](https://github.com/Microsoft/ChakraCore/pull/1198)
- Enable [Symbol.hasInstance](http://www.ecma-international.org/ecma-262/6.0/#sec-symbol.hasinstance)
under experimental flag [#1063](https://github.com/Microsoft/ChakraCore/pull/1063)

#### Performance
- Optimize creation of Heap arguments object
([`91e0e91`](https://github.com/Microsoft/ChakraCore/commit/91e0e91288ecadcfc01a41f2f0c7e878d2f3ee1a))
- Add fastpath for when Object.hasOwnProperty returns true
[#1449](https://github.com/Microsoft/ChakraCore/pull/1449)
- Enable script function inlining in jitted loop bodies
[#1182](https://github.com/Microsoft/ChakraCore/pull/1182)

#### JSRT
- JSRT Debugging APIs (experimental)
[#926](https://github.com/Microsoft/ChakraCore/pull/926)
- JSRT Module API (experimental)
[#1254](https://github.com/Microsoft/ChakraCore/pull/1254)

#### Test
- Introduce C++ unit testing mechanism using Catch
[#1224](https://github.com/Microsoft/ChakraCore/pull/1224)

## ChakraCore 1.2

### [v1.2.3](https://github.com/Microsoft/ChakraCore/releases/tag/v1.2.3)

This patch release of ChakraCore 1.2 includes the following security fixes:

- Change to address CVE-2016-7287,CVE-2016-7286,CVE-2016-7288,CVE-2016-7296
[#2230](https://github.com/Microsoft/ChakraCore/pull/2230)

### [v1.2.2](https://github.com/Microsoft/ChakraCore/releases/tag/v1.2.2)

This patch release of ChakraCore 1.2 includes the following security fixes:

- Change to address CVE-2016-7200, CVE-2016-7201, CVE-2016-720, CVE-2016-7203,
CVE-2016-7208, CVE-2016-7240, CVE-2016-7241, CVE-2016-7242, CVE-2016-7243
[#1942](https://github.com/Microsoft/ChakraCore/pull/1982)

### [v1.2.1](https://github.com/Microsoft/ChakraCore/releases/tag/v1.2.1)

This patch release of ChakraCore 1.2 includes the following security fixes:

- Fixed Address deref issue
[#1530](https://github.com/Microsoft/ChakraCore/pull/1530)
- Combined fixes for CVE-2016-3350, CVE-2016-3377 and a defense in depth change in the CustomHeap
([`24c4d7d`](https://github.com/Microsoft/ChakraCore/commit/24c4d7df8199b27d360323ce3be1d7959fd918eb))
- Changes addressing CVE_2016-3382, CVE-2016-3385, CVE-2016-3386, CVE-2016-3389, CVE-2016-3390,
CVE-2016-7189, and a mitigation of a CFG bypass.
([`f05c42e`](https://github.com/Microsoft/ChakraCore/commit/f05c42e64c3b2d057ae1a52fe1917af26c9f2737))

### [v1.2.0](https://github.com/Microsoft/ChakraCore/releases/tag/v1.2.0.0)

- Turn support for [ES2015 Destructuring Assignment](http://www.ecma-international.org/ecma-262/6.0/index.html) on by default
- Turn support for [ES2015 Default Parameters](http://www.ecma-international.org/ecma-262/6.0/index.html) on by default
- Turn support for the proposed ECMAScript [Exponentiation Operator](https://github.com/rwaldron/exponentiation-operator) on by default
- Enable proposed ECMAScript [Async Functions](https://github.com/tc39/ecmascript-asyncawait) behind an experimental flag
- Enable [ES2015 Modules](http://www.ecma-international.org/ecma-262/6.0/index.html) behind an experimental flag
- Includes multiple changes to reduce memory consumption
