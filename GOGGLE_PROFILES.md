# Brave Goggle Profiles

This document describes the available search profiles for Brave Goggle filtering, with curated source lists for different use cases.

## Profile Format

Each profile contains:
- **i** (include): Comma-separated list of preferred domains
- **e** (exclude): Comma-separated list of domains to deprioritize

## Available Profiles

### Profile: dd (Developer Documentation)

**Purpose:** Technical development, coding, cloud infrastructure, and AI/ML research

**Included Sources (24 domains):**
```
developer.mozilla.org
aws.amazon.com
cloud.google.com
learn.microsoft.com
docs.docker.com
kubernetes.io
blog.cloudflare.com
netflixtechblog.com
engineering.fb.com
eng.uber.com
stripe.com
slack.engineering
dropbox.tech
airbnb.tech
linkedin.engineering
github.blog
shopify.engineering
doordash.engineering
arxiv.org
openai.com
anthropic.com
deepmind.com
ai.googleblog.com
hai.stanford.edu
mit.edu
```

**Excluded Sources (13 domains):**
```
medium.com
geeksforgeeks.org
w3schools.com
tutorialspoint.com
javatpoint.com
dev.to
hackernoon.com
towardsdatascience.com
analyticsvidhya.com
kdnuggets.com
machinelearningmastery.com
```

**Use Cases:**
- Official documentation lookups
- Cloud infrastructure research
- Engineering blog insights
- AI/ML research papers

---

### Profile: d2 (Business, Finance, News & Policy)

**Purpose:** Business strategy, financial research, news, and policy insights

**Included Sources (25 domains):**
```
mckinsey.com
bcg.com
bain.com
hbr.org
a16z.com
stratechery.com
lennysnewsletter.com
productschool.com
firstprinciples.org
notboring.co
sequoiacap.com
benchmark.com
economist.com
ft.com
reuters.com
apnews.com
livemint.com
thehindu.com
indianexpress.com
bloomberg.com
wsj.com
niti.gov.in
prsindia.org
rbi.org.in
sebi.gov.in
```

**Excluded Sources (13 domains):**
```
forbes.com
entrepreneur.com
inc.com
businessinsider.com
indiatimes.com
ndtv.com
timesofindia.com
zeenews.india.com
opindia.com
scroll.in
thewire.in
```

**Use Cases:**
- Business strategy research
- Financial market analysis
- Policy and regulatory updates
- Government publication research
- High-quality news sources

---

## JSON Configuration

The complete profiles configuration:

```json
{
  "dd": "i=developer.mozilla.org,aws.amazon.com,cloud.google.com,learn.microsoft.com,docs.docker.com,kubernetes.io,blog.cloudflare.com,netflixtechblog.com,engineering.fb.com,eng.uber.com,stripe.com,slack.engineering,dropbox.tech,airbnb.tech,linkedin.engineering,github.blog,shopify.engineering,doordash.engineering,arxiv.org,openai.com,anthropic.com,deepmind.com,ai.googleblog.com,hai.stanford.edu,mit.edu&e=medium.com,geeksforgeeks.org,w3schools.com,tutorialspoint.com,javatpoint.com,dev.to,medium.com,hackernoon.com,towardsdatascience.com,analyticsvidhya.com,kdnuggets.com,machinelearningmastery.com",
  "d2": "i=mckinsey.com,bcg.com,bain.com,hbr.org,a16z.com,stratechery.com,lennysnewsletter.com,productschool.com,firstprinciples.org,notboring.co,sequoiacap.com,benchmark.com,economist.com,ft.com,reuters.com,apnews.com,livemint.com,thehindu.com,indianexpress.com,bloomberg.com,wsj.com,niti.gov.in,prsindia.org,rbi.org.in,sebi.gov.in&e=forbes.com,entrepreneur.com,inc.com,businessinsider.com,indiatimes.com,ndtv.com,timesofindia.com,zeenews.india.com,opindia.com,scroll.in,thewire.in"
}
```

---

## Usage

These profiles can be used to:
1. Create filtered search experiences for different domains
2. Configure Brave Goggle multi-profile support
3. Restrict searches to curated domain lists per category
4. Exclude low-quality or off-topic sources

---

## Profile Statistics

| Profile | Included Sources | Excluded Sources | Use Case |
|---------|------------------|------------------|----------|
| dd | 25 | 13 | Developer & Technical |
| d2 | 25 | 13 | Business & Finance |
| **Total** | **50** | **26** | **Multi-domain coverage** |

---

## Notes

- Profiles prioritize official documentation and expert sources
- Excluded domains are deprioritized but not completely blocked
- Included domains are boosted in search ranking
- Profiles can be combined or extended for specific needs
