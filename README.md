<!-- ===================== HEADER ===================== -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:1e3a8a,100:38bdf8&height=220&section=header&text=Eslam%20Ahmed&fontSize=56&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Java%20Backend%20Engineer%20%7C%20Codeforces%20Expert%20%7C%20Performance%20%26%20Concurrency&descAlignY=58&descSize=16" width="100%" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=1000&color=38BDF8&center=true&vCenter=true&width=780&lines=Building+High-Throughput+Enterprise+Backend+Systems;800ms+%E2%86%92+10ms+%7C+2.5x+Message-Sending+Speed;Java+8+%E2%86%92+21+%7C+WebLogic+%E2%86%92+JBoss+%7C+SOAP+%E2%86%92+REST;3500%2B+Problems+Solved+%7C+LeetCode+Top+0.8%25" alt="Typing SVG" />
</p>

<p align="center">
  <a href="mailto:eslamgamil6@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/eslam-ahmed-58b2a2247"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://codeforces.com/profile/Eslam_Ahmed"><img src="https://img.shields.io/badge/Codeforces-1868_Expert-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white" /></a>
  <a href="https://leetcode.com/u/Eslam_Ahmed/"><img src="https://img.shields.io/badge/LeetCode-2245_Top_0.8%25-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" /></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Eslam-1Ahmed&color=38bdf8&style=flat-square&label=PROFILE+VIEWS" />
</p>

---

## ⚡ `whoami`

```java
package com.eslam.profile;

public class BackendEngineer {
    private final String name      = "Eslam Ahmed";
    private final String role      = "Backend Developer @ Edafa Telecom Solutions";
    private final String location  = "Cairo, Egypt 🇪🇬";
    private final String education = "Faculty of Computers & Informatics, Zagazig University";

    public String[] getCoreFocus() {
        return new String[] {
            "Legacy Modernization  -> SOAP→REST, Java 8→21, WebLogic→JBoss, EclipseLink→Hibernate",
            "Concurrency & Safety  -> Race conditions, idempotency, duplicate-free messaging",
            "Performance           -> Deep pagination fix: 800ms → 10ms, 2.5x sending speed",
            "Streaming             -> CDC → Apache Kafka → Elasticsearch for live reporting"
        };
    }

    public CompetitiveProfile getAlgorithmicStats() {
        return CompetitiveProfile.builder()
            .problemsSolved("3,500+")
            .codeforces("Expert (Max 1868)")
            .leetCode("Max 2245 (Top 0.8% Globally)")
            .achievements("ACPC 2023 Qualifier", "ECPC Problem Setter")
            .build();
    }
}
```

---

## 🔥 Production Bugs I've Killed

| 🐛 Problem | 🛠️ Fix | 📈 Result |
|:---|:---|:---|
| Campaigns slowing down over time | OFFSET pagination → cursor-based pagination + composite index | **~800ms → 10ms**, **2.5x** sending speed |
| Duplicate campaigns on server timeouts | Unique transaction-ID validation across dual backend servers | **Zero** duplicate campaigns |
| Pause/resume race condition | Bound each contact to its own list instead of shared mutable state | Correct concurrent batches |
| Re-sending after campaign resume | Persisted filtered-out contacts to compute exact restart offset | **No** repeated messages |
| Legacy SOAP clients | JSON + XML served from the same REST endpoints | **Zero** breaking changes |

<details>
<summary><b>👀 See the pagination fix</b></summary>

```diff
- SELECT * FROM contacts
-  WHERE list_id = :listId
-  ORDER BY contact_id
-  OFFSET :offset ROWS FETCH NEXT :size ROWS ONLY;   -- scans & discards every earlier row

+ SELECT * FROM contacts
+  WHERE list_id = :listId
+    AND contact_id > :lastSeenId                   -- jumps straight to the cursor
+  ORDER BY contact_id
+  FETCH NEXT :size ROWS ONLY;
+ -- backed by a composite index on (list_id, contact_id)
```

</details>

---

## 🏗️ Real-Time Analytics Pipeline (PoC)

```mermaid
flowchart LR
    A[(SMS Logs DB)] -->|Change Data Capture| B[CDC Connector]
    B --> C[[Apache Kafka]]
    C --> D[(Elasticsearch)]
    D --> E[📊 Live Statistical Reports]
```

---

## 🛠️ Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,cpp,spring,hibernate,mysql,kafka,elasticsearch&perline=7" />
  <br/><br/>
  <img src="https://skillicons.dev/icons?i=docker,maven,git,github,postman,linux,ubuntu&perline=7" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Oracle_DB-F80000?style=flat-square&logo=oracle&logoColor=white" />
  <img src="https://img.shields.io/badge/Jakarta_EE-F7901E?style=flat-square&logo=eclipse&logoColor=white" />
  <img src="https://img.shields.io/badge/JBoss_/_WildFly-CC0000?style=flat-square&logo=redhat&logoColor=white" />
  <img src="https://img.shields.io/badge/WebLogic-F80000?style=flat-square&logo=oracle&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" />
  <img src="https://img.shields.io/badge/REST_/_SOAP-38BDF8?style=flat-square" />
</p>

---

## 🏆 Competitive Programming

<table>
<tr>
<td width="50%" valign="top">

**📊 Ratings**
- 🔵 Codeforces **Expert** — Max **1868**
- 🟠 LeetCode **2245** — **Top 0.8%** globally
- 🧩 **3,500+** problems solved

</td>
<td width="50%" valign="top">

**🥇 Highlights**
- ✍️ **Problem Setter** — ECPC Qualification Round
- 🌍 **ACPC 2023** Qualifier (57th / 250+ in ECPC)
- 🥈 **2nd** — CodeChef Starters 57 (Div. 3)
- 🎯 **Round 2** — Meta Hacker Cup 2022

</td>
</tr>
</table>

> 👨‍🏫 Trained **50+** students and led **20+** sessions on advanced data structures & competitive programming.

---

## 📊 GitHub Stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=Eslam-1Ahmed&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&bg_color=0f172a&title_color=38bdf8&icon_color=38bdf8" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Eslam-1Ahmed&layout=compact&theme=tokyonight&hide_border=true&bg_color=0f172a&title_color=38bdf8" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Eslam-1Ahmed&theme=tokyonight&hide_border=true&background=0f172a&ring=38bdf8&fire=38bdf8&currStreakLabel=38bdf8" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Eslam-1Ahmed&bg_color=0f172a&color=38bdf8&line=1e3a8a&point=ffffff&area=true&hide_border=true" width="100%" />
</p>

---

<p align="center">
  <b>💬 Let's talk backend systems, concurrency, or a tough algorithm problem.</b>
</p>

<!-- ===================== FOOTER ===================== -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:38bdf8,50:1e3a8a,100:0f172a&height=120&section=footer" width="100%" />
</p>
