<div align="center">

<img src="assets/banner.svg" width="100%" alt="TEAM JACKAL · SoftBank Hackathon 2026 Finals" />

### SoftBank Hackathon 2026 — Finals

**TEAM JACKAL**

### Beyond Lock-In
**Frictionless Cloud Management Across Platforms**

운영 중인 Stateful 애플리케이션을 **클라우드의 경계를 넘어 안전하게 이전하는**  
**AI 기반 멀티클라우드 마이그레이션 플랫폼**

<br />

<img src="https://img.shields.io/badge/SoftBank_Hackathon-2026_Finals-4B1766?style=for-the-badge" alt="SoftBank Hackathon 2026 Finals" />
<img src="https://img.shields.io/badge/TEAM-JACKAL-1F2937?style=for-the-badge" alt="Team Jackal" />
<img src="https://img.shields.io/badge/BEYOND-LOCK--IN-7C3AED?style=for-the-badge" alt="Beyond Lock-In" />

<br />
<br />

**Analyze · Adapt · Validate · Provision · Migrate**

</div>

<br />


## Technology Stack

<div align="center">

**Application & API**

<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
<img src="https://img.shields.io/badge/React-149ECA?style=for-the-badge&logo=react&logoColor=white" alt="React" />
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
<img src="https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white" alt="Pydantic" />

<br />

**Migration Workflow Orchestration**

<img src="https://img.shields.io/badge/Temporal-101010?style=for-the-badge&logo=temporal&logoColor=white" alt="Temporal" />

<br />

**Cloud & Target Environments**

<img src="https://img.shields.io/badge/AWS-EKS-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS EKS" />
<img src="https://img.shields.io/badge/Google_Cloud-GKE-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" alt="Google Cloud GKE" />
<img src="https://img.shields.io/badge/On--premises-K3s-FFC61C?style=for-the-badge&logo=k3s&logoColor=181818" alt="On-premises K3s" />

<br />

**Workload Runtime & Deployment**

<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white" alt="Helm" />

<br />

**Infrastructure & Private Connectivity**

<img src="https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform" />
<img src="https://img.shields.io/badge/WireGuard-88171A?style=for-the-badge&logo=wireguard&logoColor=white" alt="WireGuard" />

<br />

**Data & Artifacts**

<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/Amazon_S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white" alt="Amazon S3" />
<img src="https://img.shields.io/badge/Amazon_ECR-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="Amazon ECR" />

<br />

</div>
<br />


## Repositories

| 저장소 | 역할 |
| :--- | :--- |
| [cloud-migration-platform](https://github.com/SoftBank-Hackathon-2026-Team-Jackal/cloud-migration-platform) | 이전 플랫폼 본체. 분석, 이미지 빌드, 샌드박스 검증, 배포 계획·승인, 온프레미스 Agent, 데이터 복제, 트래픽 전환을 담당하는 API와 Temporal 워커 |
| [cloud-migration-web](https://github.com/SoftBank-Hackathon-2026-Team-Jackal/cloud-migration-web) | 사용자가 이전을 시작하고 단계별 진행 상황을 보고 승인하는 웹 화면 |
| [demo-app](https://github.com/SoftBank-Hackathon-2026-Team-Jackal/demo-app) | 데모에서 옮기는 원본 앱. 메시지마다 어느 환경과 DB가 처리했는지 남기는 채팅 앱 |
| [demo-application](https://github.com/SoftBank-Hackathon-2026-Team-Jackal/demo-application) | 초기 데모용 원본 앱과 시각화 웹. 현재 데모는 demo-app을 사용 |
| [Softbank-Hackathon-2026-Finals](https://github.com/SoftBank-Hackathon-2026-Team-Jackal/Softbank-Hackathon-2026-Finals) | 대회 자료, 설계 메모, PoC 기록 |

<br />

## Workflow

<div align="center">
  <img src="assets/workflow.svg" width="100%" alt="이전 한 건의 흐름: 분석, 이미지 빌드, 샌드박스 검증, 이전 계획, 승인, 구축, 데이터 복제, DB 전환, 트래픽 전환, 완료" />
</div>

운영 중인 EKS의 앱과 PostgreSQL을 분석해 이미지를 만들고, 격리된 샌드박스에서 먼저 검증합니다. 대상 환경에 맞춘 배포 계획을 사람이 승인하면 배포하고, 데이터를 복제한 뒤 짧은 쓰기 중단으로 DB를 전환하고 트래픽을 단계적으로 옮깁니다. 이 과정은 Temporal 워크플로우 하나로 이어지며, 자세한 내용은 [플랫폼 README](https://github.com/SoftBank-Hackathon-2026-Team-Jackal/cloud-migration-platform#readme)에 있습니다.

<br />

<div align="center">
  <img src="assets/clips/01-data-migration.gif" width="49%" alt="데이터 복제" />
  <img src="assets/clips/02-db-cutover.gif" width="49%" alt="DB 전환" />
  <img src="assets/clips/03-traffic-shift.gif" width="98%" alt="트래픽 전환" />
  <br />
  <sub>데이터 복제 · DB 전환 · 트래픽 전환 (웹 화면, 목업 데이터로 캡처)</sub>
</div>

<br />

## Meet Team Jackal

<div align="center">

**One Team. One Mission. Beyond Lock-In.**

<table>
  <tr>
    <td align="center" width="25%">
      <a href="https://github.com/soulee-dev"><img src="https://avatars.githubusercontent.com/u/12353597?s=120&v=4" width="84" alt="soulee-dev" /></a><br />
      <a href="https://github.com/soulee-dev"><b>@soulee-dev</b></a><br />
      <sub>Team Lead</sub>
    </td>
    <td align="center" width="25%">
      <a href="https://github.com/ikellllllll"><img src="https://avatars.githubusercontent.com/u/73003499?s=120&v=4" width="84" alt="ikellllllll" /></a><br />
      <a href="https://github.com/ikellllllll"><b>@ikellllllll</b></a>
    </td>
    <td align="center" width="25%">
      <a href="https://github.com/gumtiket"><img src="https://avatars.githubusercontent.com/u/169352115?s=120&v=4" width="84" alt="gumtiket" /></a><br />
      <a href="https://github.com/gumtiket"><b>@gumtiket</b></a>
    </td>
    <td align="center" width="25%">
      <a href="https://github.com/kmsdevdata-sketch"><img src="https://avatars.githubusercontent.com/u/241533267?s=120&v=4" width="84" alt="kmsdevdata-sketch" /></a><br />
      <a href="https://github.com/kmsdevdata-sketch"><b>@kmsdevdata-sketch</b></a>
    </td>
  </tr>
</table>

<br />

<a href="https://github.com/orgs/SoftBank-Hackathon-2026-Team-Jackal/repositories">
  <img src="https://img.shields.io/badge/Explore_Our_Repositories-181717?style=for-the-badge&logo=github&logoColor=white" alt="Explore our repositories" />
</a>

<br />
<br />


</div>
