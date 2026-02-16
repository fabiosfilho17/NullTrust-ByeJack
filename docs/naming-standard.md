===============================================================
# Naming Standard
===============================================================
- Format:
| prefix | env> | type | role/team | id |

- prefix: zt (zero trust lab)
- env: lab (ou dev for further)
- type: usr, adm, bg, grp, dev, app, stg
- role/team: law, par, it, fin, ops, etc.
- id: shortname
  
===============================================================
## Exemple
===============================================================
### - Contas administrativas
Bootstrap:
<i>zt-lab-adm-bootstrap </i>(I'm using my personal account used to create the Azure Tenant)

Break-glass:

<i>zt-lab-bg-01</i>
<i>zt-lab-bg-02</i>

---------------------------------------------------------------
### - Office users
---------------------------------------------------------------
<b>Lawers:</b>

<i>zt-lab-usr-law-01</i>

<i>zt-lab-usr-law-02</i>

<b>Paralegal/assistente:</b>

<i>zt-lab-usr-par-01</i>

<b>Financial:</b>

<i>zt-lab-usr-fin-01</i>

<b>TI:</b>

<i>zt-lab-usr-it-01</i>

<b>Contractor :</b>

<i>zt-lab-usr-ctr-01</i>

<b>Groups</b> (useful for conditional access)

<i>zt-lab-grp-lawyers</i>

<i>zt-lab-grp-paralegals</i>

<i>zt-lab-grp-finance</i>

<i>zt-lab-grp-it</i>

<i>zt-lab-grp-contractors</i>

<i>zt-lab-grp-privileged</i> (to group who has high level credentials)

<i>zt-lab-grp-breakglass-exempt</i> (only for document)

--------------------------------------------------------------------------
### - Resources
--------------------------------------------------------------------------

<b>Storage (Blob): </b>

<i>ztlablawdocs001</i> (case sensitive no hifen)

<b>Web app: </b>

zt-lab-app-case-mgmt

<b>Resource group: </b>

<i>zt-lab-rg-core</i>
