---
layout: page
title: Funding and Partners
---

<style>
/* Logo wall: every mark sits in an identical centred box and is scaled to fit,
   so wordmarks and square seals read as one uniform row. Never crop a logo. */
.logo-row {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 1.5rem 2rem;
  margin: 1.5rem 0 2rem;
  padding: 0;
  list-style: none;
}
.logo-row .logo {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 220px;
  height: 80px;
}
.logo-row .logo img {
  max-width: 100%;
  max-height: 100%;
  width: auto;
  height: auto;
  object-fit: contain;
}

/* Funding entries: fixed logo column keeps every description on the same left edge. */
.funder {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  margin: 1.75rem 0;
}
.funder-logo {
  flex: 0 0 150px;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 80px;
}
.funder-logo img {
  max-width: 100%;
  max-height: 100%;
  width: auto;
  height: auto;
  object-fit: contain;
}
.funder-text { flex: 1 1 auto; }

@media (max-width: 38rem) {
  .logo-row .logo { width: 45%; height: 64px; }
  .funder { flex-direction: column; align-items: flex-start; gap: 0.75rem; }
  .funder-logo { flex: 0 0 auto; justify-content: flex-start; height: 64px; }
}
</style>

## **UW Partners**

<div class="logo-row">
  <a class="logo" href="https://soc.washington.edu/">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/uw-dept-logo-sociology-horizontal.png" alt="UW Department of Sociology">
  </a>
  <a class="logo" href="https://csde.washington.edu/">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/CSDElogo.png" alt="Center for Studies in Demography and Ecology">
  </a>
  <a class="logo" href="https://escience.washington.edu/">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/eScience.png" alt="UW eScience Institute">
  </a>
</div>

---

## **King County Community Partners**

<div class="logo-row">
  <a class="logo" href="https://kcrha.org/">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/kcrhalogo.png" alt="King County Regional Homelessness Authority">
  </a>
  <a class="logo" href="https://etsreach.org">
    <img src="https://etsreach.org/wp-content/themes/reach/dist/images/logo.png" alt="Evergreen Treatment Services REACH">
  </a>
</div>

---

## **Funding**

<div class="funder">
  <div class="funder-logo">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/uw-dept-logo-population-health-initiative-horizontal.png" alt="UW Population Health Initiative">
  </div>
  <div class="funder-text">
    <a href="https://www.washington.edu/populationhealth/2024/06/06/initiative-announces-awardees-of-spring-quarter-2024-tier-3-pilot-research-grants/">Population Health Initiative Tier 2 and Tier 3 Grants</a>
  </div>
</div>

<div class="funder">
  <div class="funder-logo">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/NSF_Official_logo_High_Res_1200ppi.png" alt="National Science Foundation">
  </div>
  <div class="funder-text">
    <a href="https://www.nsf.gov/awardsearch/showAward?AWD_ID=2142964&amp;HistoricalAwards=false">NSF CAREER Grant #SES-2142964</a>
  </div>
</div>

<div class="funder">
  <div class="funder-logo">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/img/NIH_Master_Logo_Vertical_2Color.png" alt="National Institutes of Health">
  </div>
  <div class="funder-text">
    <a href="https://csde.washington.edu/about/acknowledge-csde/">Eunice Kennedy Shriver National Institute of Child Health and Human Development research infrastructure grant, P2C HD042828, to the Center for Studies in Demography &amp; Ecology at the University of Washington</a>
  </div>
</div>

The content is solely the working group's responsibility and does not necessarily represent the official NIH or National NSF views.
