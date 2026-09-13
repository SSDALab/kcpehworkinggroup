---
layout: page
title: Projects
---

<style>
.project {
  display: flex;
  align-items: flex-start;
  gap: 1.5rem;
  padding: 1.25rem 0;
  border-top: 1px solid #eceaf1;
}
.project:first-of-type { border-top: 0; padding-top: 0.5rem; }
.project-img {
  flex: 0 0 150px;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 82px;
}
.project-img img {
  max-width: 100%;
  max-height: 100%;
  width: auto;
  height: auto;
  object-fit: contain;
}
.project-body { flex: 1 1 auto; }
.project-body h3 { margin: 0 0 0.15rem; font-size: 1.05rem; }
.project-body p { margin: 0.35rem 0 0; }
.project-meta { color: #6f6f7a; font-size: 0.85rem; }
.project-links { font-size: 0.88rem; }

@media (max-width: 32rem) {
  .project { flex-direction: column; gap: 0.75rem; }
  .project-img { flex: 0 0 auto; justify-content: flex-start; height: 64px; }
}
</style>

<div class="project">
  <div class="project-img">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/kcrhalogo.png" alt="King County Regional Homelessness Authority">
  </div>
  <div class="project-body">
    <h3>UW/KCRHA Point-in-Time Count</h3>
    <p class="project-meta">2022–present · with KCRHA, ETS REACH, WHEEL/SHARE, and King County Public Health</p>
    <p>Replacing the visual street census with respondent-driven sampling, a peer-referral method that
    produces quasi-probability estimates of the unsheltered population. Piloted in King County in 2022,
    refined in 2023, and used for the formal HUD count from 2024.</p>
    <p class="project-links"><a href="https://academic.oup.com/aje/advance-article-abstract/doi/10.1093/aje/kwae342/7749332">Almquist et al. (2025), <em>American Journal of Epidemiology</em></a> · <a href="https://uwescience.github.io/DSSG2024_understanding_homelessness/">2023 Understanding Homelessness project</a></p>
  </div>
</div>

<div class="project">
  <div class="project-img">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/NSF_Official_logo_High_Res_1200ppi.png" alt="National Science Foundation">
  </div>
  <div class="project-body">
    <h3>NSF CAREER: Networks and Demographics of People Experiencing Homelessness</h3>
    <p class="project-meta">2022–2027 · NSF Social, Behavioral &amp; Economic Sciences · $500,000</p>
    <p>Measuring and modelling the multi-modal networks and demographics of people experiencing
    homelessness, and building the statistical methods that make network-based enumeration practical.</p>
    <p class="project-links"><a href="https://www.nsf.gov/awardsearch/showAward?AWD_ID=2142964&amp;HistoricalAwards=false">NSF Award #SES-2142964</a></p>
  </div>
</div>

<div class="project">
  <div class="project-img">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/reach-logo.png" alt="Evergreen Treatment Services REACH">
  </div>
  <div class="project-body">
    <h3>ETS REACH Street Outreach Data</h3>
    <p class="project-meta">with Evergreen Treatment Services REACH</p>
    <p>Using longitudinal street-outreach records from Seattle to study where unsheltered people
    actually live and where they go afterwards — encampment siting relative to amenities, and housing
    and movement outcomes following encampment clearances.</p>
    <p class="project-links"><a href="https://doi.org/10.1016/j.cities.2025.106348">Sutton, Walker, Hagopian &amp; Almquist (2025), <em>Cities</em></a> · <a href="https://arxiv.org/abs/2608.04076">Morande et al., encampment clearances</a></p>
  </div>
</div>

<div class="project">
  <div class="project-img">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/la-youth-count-logo.png" alt="LA Youth Count">
  </div>
  <div class="project-body">
    <h3>LA Youth Count</h3>
    <p class="project-meta">Los Angeles County</p>
    <p>Extending peer-referral sampling to youth homelessness, with young people themselves recruiting
    participants rather than being counted by canvassers.</p>
    <p class="project-links"><a href="https://imprintnews.org/top-stories/l-a-county-tests-new-approach-to-counting-homeless-youth-relying-on-youth-themselves/276177">The Imprint</a> · <a href="https://nextcity.org/urbanist-news/la-county-tests-new-approach-counting-homeless-youth-sampling">Next City</a></p>
  </div>
</div>

<div class="project">
  <div class="project-img">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/uw-dept-logo-population-health-initiative-horizontal.png" alt="UW Population Health Initiative">
  </div>
  <div class="project-body">
    <h3>Community-driven Enumeration and Needs Assessment</h3>
    <p class="project-meta">UW Population Health Initiative · Tier 2 pilot 2022–2023 ($106,822) and 2024–2026 ($217,593)</p>
    <p>Developing higher-frequency enumeration and needs-assessment methods built around the people and
    organisations already doing outreach.</p>
    <p class="project-links"><a href="https://www.washington.edu/populationhealth/2024/06/06/initiative-announces-awardees-of-spring-quarter-2024-tier-3-pilot-research-grants/">Population Health Initiative award</a></p>
  </div>
</div>
