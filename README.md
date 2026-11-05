<!-- Animated Header Banner -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e3a8a&height=200&section=header&text=Eslam%20Ahmed&fontSize=50&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Java%20Backend%20Engineer%20%7C%20Codeforces%20Expert%20(1868)%20%7C%20System%20Optimization&descAlignY=58&descSize=16" width="100%" />
</p>

<!-- Typing SVG -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=1000&color=38BDF8&center=true&vCenter=true&width=750&lines=Building+High-Throughput+Enterprise+Backend+Systems;Java+8+to+21+%7C+Spring+Boot+%7C+Jakarta+EE+%7C+Hibernate;3500%2B+Algorithmic+Problems+Solved+%7C+LeetCode+Top+0.8%25;Optimizing+Queries%2C+Concurrency+%26+Real-Time+Pipelines" alt="Typing SVG" />
</p>

<!-- Social & Competitive Links -->
<p align="center">
  <a href="mailto:eslamgamil6@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://www.linkedin.com/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://codeforces.com/profile/Eslam_Ahmed">
    <img src="https://img.shields.io/badge/Codeforces-1868_(Expert)-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white" alt="Codeforces" />
  </a>
  <a href="https://leetcode.com/">
    <img src="https://img.shields.io/badge/LeetCode-2245_(Top_0.8%25)-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" />
  </a>
</p>

---

### ⚡ Who Am I?

```java
package com.eslam.profile;

public class BackendEngineer {
    private final String name = "Eslam Ahmed";
    private final String role = "Backend Developer @ Edafa Telecom Solutions";
    private final String location = "Cairo, Egypt";
    private final String education = "B.Sc. in Computer Science, Zagazig University";

    public String[] getCoreFocus() {
        return new String[] {
            "Legacy Modernization (SOAP -> REST, Java 8 -> 21, WebLogic -> JBoss, EclipseLink -> Hibernate)",
            "High-Concurrency, Database-Level Idempotency & Race Condition Resolution",
            "Query & Deep Pagination Optimization (800ms -> 10ms | 2.5x Throughput Boost)",
            "Real-Time Streaming Pipelines (Oracle/MySQL -> CDC -> Apache Kafka -> ELK)"
        };
    }

    public CompetitiveProfile getAlgorithmicStats() {
        return CompetitiveProfile.builder()
            .problemsSolved("3,500+")
            .codeforces("Expert (Max Rating: 1868)")
            .leetCode("Max Rating: 2245 (Top 0.8% Globally)")
            .achievements(new String[]{"ACPC 2023 Regional Finalist", "ECPC Problem Setter"})
            .build();
    }
}
