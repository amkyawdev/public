# Social Circle - အပျော်တမ်း စကားပြော အသိုင်းအဝိုင်း

**JSON ဖြင့် ဖန်တီးထားသော လူမှုကွန်ရက် စကားပြော အက်ပ်**

![Version](https://img.shields.io/badge/version-1.0-blue)
![License](https://img.shields.io/badge/license-MIT-gray)
![Platform](https://img.shields.io/badge/platform-Web-blue)

> အချက်အလက်သိမ်းဆည်းမှုအားလုံးကို JSON နှင့် localStorage ဖြင့် စီမံထားသော မိုဘိုင်း-ဖော်ရွေ ဆိုရှယ်အက်ပ်လီကေးရှင်း

---

## 📖 အကြောင်းအရာ (Overview)

Social Circle သည် အသုံးပြုသူများအကြား **ပို့စ်များမျှဝေခြင်း**၊ **အများပြည်သူချတ်ခန်း** နှင့် **ကိုယ်ရေးအချက်အလက်များ** ကို JSON data system ဖြင့် စီမံထားသော အပျော်တမ်း ဆိုရှယ်အက်ပ်တစ်ခုဖြစ်သည်။

### ✨ အဓိက လုပ်ဆောင်ချက်များ (Features)

| လုပ်ဆောင်ချက် | ဖော်ပြချက် |
|---|---|
| 🔐 **အကောင့်ဝင်ခြင်း/မှတ်ပုံတင်ခြင်း** | JSON user system ဖြင့် signup/login, ဆက်ရှင်သိမ်းဆည်းခြင်း |
| 🏠 **ပင်မစာမျက်နှာ (Main Feed)** | အသုံးပြုသူအားလုံး၏ ပို့စ်များကို အချိန်နှင့်တပြေးညီ ကြည့်ရှုနိုင် |
| 🌍 **အများပြည်သူပို့စ်များ** | ကမ္ဘာလုံးဆိုင်ရာ ပို့စ်များ ဖန်တီးခြင်းနှင့် ကြည့်ရှုခြင်း |
| 💬 **အများပြည်သူချတ်ခန်း** | အချိန်နှင့်တပြေးညီ စကားပြောဆိုခြင်း (JSON message store) |
| 👤 **ကိုယ်ရေးအချက်အလက်စာမျက်နှာ** | JSON data ကို အပြည့်အစုံကြည့်ရှုနိုင်ပြီး bio ပြင်ဆင်နိုင် |
| 🍔 **Hamburger Menu** | ဘေးဘား menu မှ စာမျက်နှာအားလုံးသို့ လွယ်ကူစွာသွားနိုင် |

### 🎨 အရောင်အဆင်း (Color Scheme)

- **အပြာ (Primary Blue):** `#1E5AF7` - ခလုတ်များ၊ link များ၊ အဓိက accent
- **မီးခိုး (Gray):** `#F8FAFE`, `#E9EDF2` - နောက်ခံ၊ ဘောင်များ၊ စကားပြော bubbles

---

## 🗄️ JSON Data System အကြောင်း

ဤအက်ပ်သည် **backend server မလိုအပ်ဘဲ** သုံးစွဲသူ၏ browser အတွင်းရှိ `localStorage` တွင် JSON format ဖြင့် အချက်အလက်အားလုံးကို သိမ်းဆည်းသည်။

### JSON Data Structure (အချက်အလက်ပုံစံ)

```json
// usersDB - အသုံးပြုသူများစာရင်း
[
  {
    "id": "u1",
    "username": "alice",
    "password": "123",
    "bio": "Exploring the world 🌍 | Blue lover"
  }
]

// postsDB - ပို့စ်များ
[
  {
    "id": "p1700000000000",
    "userId": "u1",
    "username": "alice",
    "content": "Hello everyone!",
    "timestamp": 1700000000000
  }
]

// chatMessages - ချတ်မက်ဆေ့ခ်ျများ
[
  {
    "id": "c1700000000000",
    "username": "alice",
    "text": "Hi there!",
    "timestamp": 1700000000000
  }
]
```

localStorage Keys များ

Key သိုလှောင်သည့်အကြောင်းအရာ
socialcircle_users အသုံးပြုသူအားလုံး၏ JSON array
socialcircle_posts ပို့စ်အားလုံး
socialcircle_chat ချတ်မက်ဆေ့ခ်ျအားလုံး
socialcircle_currentUser လက်ရှိ login ဝင်ထားသူ၏ session

---

🚀 စတင်အသုံးပြုရန် (Getting Started)

လိုအပ်ချက်များ (Prerequisites)

· ခေတ်မီ browser တစ်ခု (Chrome, Firefox, Safari, Edge)
· အင်တာနက်ချိတ်ဆက်မှု (Bootstrap Icons အတွက် ပထမတစ်ကြိမ်သာ)

အသုံးပြုနည်း (How to Use)

1. အက်ပ်ကိုဖွင့်ပါ - index.html ကို browser ဖြင့်ဖွင့်ပါ။
2. Get Started ကိုနှိပ်ပါ။
3. အကောင့်ဝင်ရန် (Login) -
   · Demo users: alice / 123 သို့ bob / 123
   · သို့မဟုတ် "Sign Up" ဖြင့် အကောင့်သစ်ဖွင့်ပါ။
4. ပင်မစာမျက်နှာ တွင် ပို့စ်များကြည့်ရှုနိုင်ပြီး "New Post" ဖြင့် ကိုယ်ပိုင်ပို့စ်တင်နိုင်ပါသည်။
5. Hamburger Menu (☰) ကိုနှိပ်၍ အခြားစာမျက်နှာများသို့ သွားနိုင်ပါသည်။
   · Public Posts - ကမ္ဘာလုံးဆိုင်ရာ ပို့စ်များ
   · Public Chat - အခြားအသုံးပြုသူများနှင့် စကားပြောဆိုရန်
   · My Profile - ကိုယ်ရေးအချက်အလက်နှင့် JSON data ကြည့်ရန်

---

📁 Project Structure (ပရောဂျက်ဖွဲ့စည်းပုံ)

ဤအက်ပ်သည် single HTML file (all-in-one) ဖြစ်သော်လည်း လက်တွေ့တည်ဆောက်လျှင်အပိုင်းများခွဲထားသည်-

```
SocialChatApp/
├── index.html          # Main entry (HTML + CSS + JS အားလုံးပါဝင်)
│
├── 📁 styles (embedded)
│   ├── Blue & Gray theme
│   ├── Responsive mobile-first CSS
│   └── Card, chat bubble, menu styling
│
├── 📁 scripts (embedded)
│   ├── JSON Storage Layer (localStorage)
│   ├── Authentication Module
│   ├── Posts & Chat CRUD
│   ├── Page Router (6 views)
│   └── UI Renderers
│
└── 📁 data (browser localStorage)
    ├── users.json (virtual)
    ├── posts.json (virtual)
    └── chat.json (virtual)
```

စာမျက်နှာ ၆ ခု (6 Pages)

1. Get Started - ကြိုဆိုမျက်နှာပြင်
2. Auth Page - Login / Signup
3. Main Page - ပင်မပို့စ်များ
4. Public Post Page - အများပြည်သူပို့စ်များ
5. Public Chat Page - အများပြည်သူစကားပြောခန်း
6. User Info Page - ကိုယ်ရေးအချက်အလက် + JSON viewer

---

🛠️ အသုံးပြုထားသော နည်းပညာများ (Tech Stack)

နည်းပညာ အသုံးပြုပုံ
HTML5 စာမျက်နှာဖွဲ့စည်းပုံ၊ modal, menu
CSS3 Blue/Gray theme, responsive design, flexbox
Bootstrap Icons icon များအတွက် (CDN)
Vanilla JavaScript အက်ပ် logic အားလုံး (no framework)
localStorage API JSON data သိုလှောင်ရန်
JSON data structure format

---

🔄 အလုပ်လုပ်ပုံ အဆင့်ဆင့် (Data Flow)

```
User Action (e.g., Create Post)
        ↓
JavaScript Function (createPost)
        ↓
Modify postsDB array
        ↓
savePosts() → localStorage.setItem()
        ↓
Re-render affected pages (Main Feed, Public Posts)
        ↓
UI updated instantly
```

---

🎯 Demo Credentials (စမ်းသုံးရန် အထောက်အထားများ)

Username Password Role
alice 123 Demo user 1
bob 123 Demo user 2

💡 စိတ်ကြိုက် အကောင့်ဖွင့်နည်း - Auth Page တွင် username နှင့် password အသစ်ဖြည့်၍ "Sign Up" နှိပ်ပါ။

---

📱 Mobile Responsive

· Container width: အများဆုံး 500px (မိုဘိုင်းလ်ပုံစံ)
· ဒက်စတော့: အလယ်ဗဟိုတွင် shadow ကျပြီး ပြသမည်
· ထိလွယ်ရှလွယ် ခလုတ်များ: လက်ချောင်းဖြင့် အလွယ်တကူနှိပ်နိုင်

---

❓ FAQs (မေးလေ့ရှိသောမေးခွန်းများ)

မေး။ ။ အင်တာနက်မပါဘဲ သုံးလို့ရလား။
ဖြေ။ ။ ပထမတစ်ကြိမ် Bootstrap Icons loading အတွက် အင်တာနက်လိုအပ်သည်။ ဒုတိယအကြိမ်မှစ၍ offline သုံးနိုင်သည် (cached)။

မေး။ ။ အချက်အလက်တွေ ဘယ်မှာသိမ်းထားလဲ။
ဖြေ။ ။ Browser ၏ localStorage တွင် JSON format ဖြင့် သိမ်းဆည်းထားသည်။

မေး။ ။ အချက်အလက်တွေ ပျက်သွားနိုင်လား။
ဖြေ။ ။ Browser data ရှင်းလျှင် (clear site data) ပျက်နိုင်သည်။ Export feature မပါသေးပါ။

မေး။ ။ အခြားအသုံးပြုသူများနှင့် real-time စကားပြောနိုင်လား။
ဖြေ။ ။ ဤဗားရှင်းသည် real-time server မပါသော်လည်း localStorage ကို အခြေခံထားသည်။ သို့သော် page refresh လုပ်ပါက အခြားသူများ၏ message များကို မြင်ရသည် (တူညီသော browser တွင်သာ)။

---

🔮 အနာဂတ်တွင် ထည့်သွင်းနိုင်သော အချက်များ (Future Improvements)

· Cloud database ချိတ်ဆက်ခြင်း (Firebase / Supabase)
· Real-time WebSocket chat
· ပို့စ်များကို Like/Comment လုပ်ခြင်း
· Profile picture အပ်လုဒ်လုပ်ခြင်း
· Dark mode support
· Data export (backup JSON)

---

📄 လိုင်စင် (License)

MIT License - မည်သူမဆို အခမဲ့အသုံးပြု၊ ပြင်ဆင်၊ မျှဝေနိုင်ပါသည်။

---

👨‍💻 Developer Note

ဤအက်ပ်သည် JSON data system ကို အခြေခံ၍ အပျော်တမ်း ဆိုရှယ်အက်ပ် တည်ဆောက်နည်းကို သရုပ်ပြရန် ရေးသားထားခြင်းဖြစ်သည်။ Backend မပါဘဲ Frontend သက်သက်ဖြင့် လုပ်ဆောင်နိုင်သော ဥပမာတစ်ခုဖြစ်သည်။

ပျော်ရွှင်စွာ စကားပြောဆိုပါ! 🎉💬

---

Built with ❤️ using HTML, CSS, JavaScript & JSON

```
