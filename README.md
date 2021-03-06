# @ngx-prism/core

[![npm version](https://badge.fury.io/js/%40ngx-prism%2Fcore.svg)](https://badge.fury.io/js/%40ngx-prism%2Fcore)
[![GitHub version](https://badge.fury.io/gh/ngx-prism%2Fcore.svg)](https://badge.fury.io/gh/ngx-prism%2Fcore)
[![Package Quality](http://npm.packagequality.com/shield/ngx-prism.svg)](http://packagequality.com/#?package=ngx-prism)
[![Known Vulnerabilities](https://snyk.io/test/npm/ngx-prism/badge.svg)](https://snyk.io/test/npm/ngx-prism)
[![GitHub issues](https://img.shields.io/github/issues/ngx-prism/core.svg)](https://github.com/ngx-prism/core/issues)
[![GitHub forks](https://img.shields.io/github/forks/ngx-prism/core.svg)](https://github.com/ngx-prism/core/network)
[![GitHub stars](https://img.shields.io/github/stars/ngx-prism/core.svg)](https://github.com/ngx-prism/core/stargazers)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/ngx-prism/core/master/LICENSE)

Angular 2+ Component of Prism a lightweight, extensible syntax highlighter, built with modern web standards in mind.

## Table of contents
* [Installation](#installation)
* [Usage](#usage)
* [Versioning](#versioning)
* [Git commit](#git-commit)
* [License](#license)
* [Donate](#donate)

## Installation

To install, run:

```bash
npm install @ngx-prism/core --save
```

## Usage

1. Import `PrismModule` into your module.
```typescript
// example.module.ts
import { NgModule } from '@angular/core';
import { CommonModule } from '@angular/common';

import { PrismModule } from './prism.component';
import { ExampleComponent } from './example.component';

@NgModule({
  declarations: [ ExampleComponent ],
  imports: [ CommonModule, PrismModule ],
  exports: [ ExampleComponent ]
})
export class ExampleModule { }
```

2. Use prism component in your example component.
```typescript
// example.component.ts
import { Component } from '@angular/core';

@Component({
  selector: 'example-component',
  template: `<prism-highlight [language]="language">{{content}}</prism-highlight>`
})
export class ExampleComponent {
  language = 'html';
  content = '<p>test</p>';
  constructor() { }
}
```


## Versioning
Semantic Versioning 2.0.0 http://semver.org/

**Given a version number MAJOR.MINOR.PATCH, increment the:**   
MAJOR version when you make incompatible API changes,  
MINOR version when you add functionality in a backwards-compatible manner, and  
PATCH version when you make backwards-compatible bug fixes.  
Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

**FAQ**   
How should I deal with revisions in the 0.y.z initial development phase?  
>The simplest thing to do is start your initial development release at 0.1.0 and then increment the minor version for each subsequent release.

How do I know when to release 1.0.0?

>If your software is being used in production, it should probably already be 1.0.0. If you have a stable API on which users have come to depend, you should be 1.0.0. If you’re worrying a lot about backwards compatibility, you should probably already be 1.0.0.

## GIT commit
- AngularJS Git Commit Message Conventions https://gist.github.com/stephenparish/9941e89d80e2bc58a153
- http://karma-runner.github.io/0.10/dev/git-commit-msg.html

## License

MIT © ngx-prism

## Donate

[Click to donate](https://donorbox.org/help-creating-open-source-software)
