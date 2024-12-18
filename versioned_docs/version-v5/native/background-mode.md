---
title: 'Native Background Mode | Cordova-Plugin-Background-Mode'
description: 'Learn about Cordova-plugin-background-mode usage. This Cordova plugin, for Ionic Native Apps, prevents the app from going to sleep while in background.'
sidebar_label: 'Background Mode'
---

import DocsCard from '@components/global/DocsCard';
import DocsButton from '@components/page/native/DocsButton';
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';
import CodeBlock from '@theme/CodeBlock';

# Background Mode

Cordova plugin to prevent the app from going to sleep while in background.
Requires Cordova plugin: cordova-plugin-background-mode. For more info about plugin, visit: https://github.com/katzer/cordova-plugin-background-mode

<p>
  <a href="https://github.com/katzer/cordova-plugin-background-mode" target="_blank" rel="noopener" className="git-link">github.com/katzer/cordova-plugin-background-mode</a>
</p>

<h2>Stuck on a Cordova issue?</h2>
<DocsCard
  className="cordova-ee-card"
  header="Don't waste precious time on plugin issues."
  href="https://ionicframework.com/sales?product_of_interest=Ionic%20Native"
>
  <div>
    <img src="/docs/icons/native-cordova-bot.png" className="cordova-ee-img" />
    <p>If you're building a serious project, you can't afford to spend hours troubleshooting. Ionic’s experts offer premium advisory services for both community plugins and premier plugins.</p>
    <DocsButton className="native-ee-detail">Contact Us Today!</DocsButton>
  </div>
</DocsCard>

<h2 id="installation">
  <a href="#installation">Installation</a>
</h2>
<Tabs
  groupId="runtime"
  defaultValue="Capacitor"
  values={[
    { value: 'Capacitor', label: 'Capacitor' },
    { value: 'Cordova', label: 'Cordova' },
    { value: 'Enterprise', label: 'Enterprise' },
  ]}
>
  <TabItem value="Capacitor">
    <CodeBlock className="language-shell">
      $ npm install cordova-plugin-background-mode {'\n'}$ npm install @awesome-cordova-plugins/background-mode {'\n'}$
      ionic cap sync
    </CodeBlock>
  </TabItem>
  <TabItem value="Cordova">
    <CodeBlock className="language-shell">
      $ ionic cordova plugin add cordova-plugin-background-mode {'\n'}$ npm install
      @awesome-cordova-plugins/background-mode {'\n'}
    </CodeBlock>
  </TabItem>
  <TabItem value="Enterprise">
    <blockquote>
      Ionic Enterprise comes with fully supported and maintained plugins from the Ionic Team. &nbsp;
      <a className="btn" href="https://ionic.io/docs/premier-plugins">Learn More</a> or if you're interested in an enterprise version of this plugin <a className="btn" href="https://ionicframework.com/sales?product_of_interest=Ionic%20Enterprise%20Engine">Contact Us</a>
    </blockquote>
  </TabItem>
</Tabs>

## Supported Platforms

- AmazonFire OS
- Android
- Browser
- iOS
- Windows

## Usage

### React

[Learn more about using Ionic Native components in React](../native-community.md#react)

### Angular

```tsx
import { BackgroundMode } from '@awesome-cordova-plugins/background-mode/ngx';

constructor(private backgroundMode: BackgroundMode) { }

...

this.backgroundMode.enable();
```