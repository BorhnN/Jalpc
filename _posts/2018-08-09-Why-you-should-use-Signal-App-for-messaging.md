<!-- # আমাদের অনলাইনে মেসেজ আদান প্রদান কতটা নিরাপদ? -->
### সিগন্যাল প্রটোকল বর্তমানে সবথেকে নিরাপদ মেসেজিং সিস্টেম

Open Whisper System এর উদ্ভাবিত Signal Protocol বর্তমানে পৃথিবীতে সবচেয়ে নিরাপদ মেসেজ আদান প্রদানের উপায়। বর্তমানে অনেকগুলো এন্ড টু এন্ড এনক্রিপশন ওয়ালা মেসেঞ্জার প্রচলিত। তবে এরা দুইটি E2E প্রটোকল ব্যবহার করে। 

1. Signal Protocol by Open Whisper System
1. MTproto by Telegram Messenger LLC

Security researcher দের অ্যানালাইসিস অনুযায়ি Signal Protocol সবচেয়ে secure এবং robust। MTproto বেশ secure হলেও গবেষকরা বেশ কয়েকটি পয়েন্টে এর সমালোচনা করে থাকেন।

### সিগন্যাল প্রোটোকল সবচেয়ে বেশি ব্যবহৃত End to End Encryption ব্যবস্থা

উপরে আমি মাত্র দুইটি E2E প্রটোকলের কথা উল্লেখ করেছি। যা যথাক্রমে Signal Messenger এবং Telegram Messenger ব্যবহার করে থাকে। তাহলে WhatsApp কী ব্যবহার করে?

উত্তর Signal Protocol

একারণেই Signal ব্যবহারকারী তেমন বেশি না হলেও সবচেয়ে বেশি ব্যবহৃত E2E system হলো Signal Protocol

আমরা তাহলে অন্যান্য মেসেঞ্জারের লিস্ট দেখি:



| অ্যাপ                                     | প্রটোকল         |
| ----------------------------------------- | --------------- |
| WhatsApp                                  | Signal Protocol |
| Facebook Messenger                        | Not E2E Secure  |
| Facebook Messenger - Secret Conversations | Signal Protocol |
| Signal Private Messenger                  | Signal Protocol |
| Telegram                                  | MTproto         |
| Google Allo                               | Not E2E Secure  |
| Google Allo - Incognito Mode              | Signal Protocol |
| Skype Chat                                | Signal Protocol |


সুতরাং পরিস্কার দেখা যাচ্ছে Telegram ব্যতিত সব জনপ্রিয় E2E মেসেজিং অ্যাপ Signal Protocol ব্যবহার করে। Google, Facebook বা Microsoft এর মতো বড় বড় টেক জায়ান্টের নতুন করে protocol তৈরি না করার কারণ Signal protocol এর robust security।

#### তাহলে আমি কেন Signal অ্যাপ ব্যবহার করব?
এখন প্রশ্ন আসতেই পারে যে Signal Protocol যদি সবচেয়ে নিরাপদ ব্যবস্থাই হয় আর WhatApp এবং Signal দুইটা অ্যাপ এ যদি একই security থাকে তাহলে আমি কেন WhatsApp ছেড়ে Signal ব্যবহার করব? আমার সব বন্ধুরা WhatsApp এ আছে অপরদিকে Signal তেমন popular না।

##### E2E মানেই সবকিছু নয়
WhatsApp E2E Encrypted হওয়া মানে শুধু এটাই আপনি যে মেসেজটি পাঠাচ্ছেন তা শুধুমাত্র যাকে পাঠাচ্ছেন সেই দেখতে পাবে। মাঝে থেকে অন্য কেউ মেসেজটি পড়তে পারবে না। যেমন WhatsApp বা Facebook। কিন্তু WhatsApp (যার মালিক Facebook Inc.) আপনার বাকি সব তথ্য দেখতে পাচ্ছে। যেমন, আপনি কাকে মেসেজ দিচ্ছেন, প্রতিদিন কতগুলো মেসেজ দেন এবং কাকে কাকে দেন, মেসেজগুলো কত ছোট বা বড়, আপনার নাম, আপনার contact এ কে কে আছে, তাদের নাম ইত্যাদি।

অপরদিকে Signal আপনার মাত্র দুইটি information তাদের সার্ভারে রাখে।


1. আপনার ফোন নম্বর
1. শেষ কবে সার্ভারের সাথে যোগাযোগ হয়েছিল 


শুধু একটুকুই। Signal এর সার্ভার জানেনা আপনার নাম, আপনার ফোনবুকে কত জন Signal ব্যবহার করে এবং তারা কে কে। ভয়ের কিছু নেই Signal app ব্যবহার করলে আপনি জানতে পারবেন আপনার ফোনবুকে কে কে Signal ব্যবহার করে সার্ভারকে আপনার ফোনবুক দেওয়া ছাড়াই।

কিন্তু কিভাবে আমরা জানি যে Signal তার ব্যবহারকারীর অন্য কোন তথ্য সংগ্রহ করে না বা জমা রাখে না?

##### Open Source
WhatsApp বা Google Allo যে Signal প্রটোকল ব্যবহার করে এটা আমরা জানি তাদের মুখের কথা থেকেই (এবং Signal Team এর  [ব্লগ post](https://signal.org/blog/whatsapp-complete/) [থেকে](https://signal.org/blog/allo/))। সাথে সতন্ত্র Security গবেষকদের রিসার্চ এর উপর নির্ভর করে আমরা নিশ্চিত হতে পারি। তবে তারা WhatsApp, Google বা Facebook সংগে কী কী তথ্য সংগ্রহ করে তা জানা অনেক কঠিন। 

অপরদিকে Signal এর প্রত্যেকটি application ই Open Source। তারমানে যে কেউ এর কোডের দিকে তাকালেই দেখতে পাবে এটা কী করে, কী কী তথ্য সংগ্রহ করে বা কী কী তথ্য জমা রাখে। এর জন্য আমাদের কারো মুখের কথায় বিশ্বাসের প্রয়োজন নেই।

এখন যদি হঠাৎ কখনো WhatsApp তাদের app থেকে Signal Protocol বাদ দিয়ে অন্যকিছু ব্যবহার করা শুরু করে বা ইচ্ছা করে কিংবা কোন ক্ষমতাধারীর (FBI, NSA বা কোন দেশের সরকার) চাপে পড়ে তাদের অ্যাাপের Signal Protocol এ দুর্বলতা নিয়ে আসে যাতে করে মেসেজগুলো পড়া যায় ([backdoor](https://en.wikipedia.org/wiki/Backdoor_(computing))) আমরা তা সহজে জানতে পারবো না। এবং backdoor ছাড়াই তারা যে পরিমান তথ্য সংগ্রহ করে এবং অন্যদের দিয়ে থাকে তা বেশ [অস্বস্তিকর](https://www.forbes.com/sites/thomasbrewster/2017/01/22/whatsapp-facebook-backdoor-government-data-request/#2e73896a1030)।

এবার আসি Telegram এ। Telegram LLC বলে থাকে যে Telegram অ্যাপটি open sourced কিন্তু তাদের কোড repo তে গেলে দেখা যায় যে আসলে তাদের কোড এর সাথে app মিলে না এবং তা সবসময়ে কয়েক মাস পিছিয়ে থাকে। Open Souce এর মানে এটা নয়। তারা Open Source নামটা ব্যবহার করে পাবলিসিটির _জন্য।_



[![ক্রিয়েটিভ কমন্স লাইসেন্স](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)  
এই লেখাটি [ক্রিয়েটিভ কমন্স অ্যাট্রিবিউশন-শেয়ার অ্যালাইক 4.0 আন্তর্জাতিক লাইসেন্সের](http://creativecommons.org/licenses/by-sa/4.0/) অধীনে লাইসেন্সকৃত।