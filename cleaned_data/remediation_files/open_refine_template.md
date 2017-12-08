# OpenRefine Template for UT Theatre Collection Playbills (migration)

---

## Prefix

```
<?xml version="1.0" encoding="UTF-8"?>
<modsCollection xmlns="http://www.loc.gov/mods/v3" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http://www.w3.org/1999/xlink" xsi:schemaLocation="http://www.loc.gov/mods/v3 http://www.loc.gov/standards/mods/v3/mods-3-5.xsd">
```

## Row Template

```
<mods>

<title><titleInfo>{{cells["title"].value}}</titleInfo></title>
{{if(isBlank(cells["abstract"].value),'', '<abstract>' + cells['abstract'].value + '</abstract>')}}
{{if(isBlank(cells['creator'].value), '', '<name'+ if(isBlank(cells['creator_URI'].value), '', ' valueURI="' + cells['creator_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['creator'].value + '</namePart>' + if(isBlank(cells['role'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['role_URI'].value + '">' + cells['role'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['creator2'].value), '', '<name'+ if(isBlank(cells['creator2_URI'].value), '', ' valueURI="' + cells['creator2_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['creator'].value + '</namePart>' + if(isBlank(cells['creator2'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['role_URI'].value + '">' + cells['role'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['creator2'].value), '', '<name'+ if(isBlank(cells['creator2_URI'].value), '', ' valueURI="' + cells['creator2_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['creator'].value + '</namePart>' + if(isBlank(cells['creator2'].value), '', '<role><roleTerm authority="marcrelator valueURI="' + cells['role_URI'].value + '">' + cells['role'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['creator3'].value), '', '<name'+ if(isBlank(cells['creator3_URI'].value), '', ' valueURI="' + cells['creator3_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['creator3'].value + '</namePart>' + if(isBlank(cells['creator3'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['role_URI'].value + '">' + cells['role'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['creator4'].value), '', '<name'+ if(isBlank(cells['creator4_URI'].value), '', ' valueURI="' + cells['creator4_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['creator4'].value + '</namePart>' + if(isBlank(cells['creator4'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['role_URI'].value + '">' + cells['role'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['creator5'].value), '', '<name'+ if(isBlank(cells['creator5_URI'].value), '', ' valueURI="' + cells['creator5_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['creator5'].value + '</namePart>' + if(isBlank(cells['creator5'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['role_URI'].value + '">' + cells['role'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['creator6'].value), '', '<name'+ if(isBlank(cells['creator6_URI'].value), '', ' valueURI="' + cells['creator6_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['creator6'].value + '</namePart>' + if(isBlank(cells['creator6'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['role_URI'].value + '">' + cells['role'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['director'].value), '', '<name'+ if(isBlank(cells['director_URI'].value), '', ' valueURI="' + cells['director_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['director'].value + '</namePart>' + if(isBlank(cells['director'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['role2_URI'].value + '">' + cells['role2'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['director2'].value), '', '<name'+ if(isBlank(cells['director2_URI'].value), '', ' valueURI="' + cells['director2_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['director2'].value + '</namePart>' + if(isBlank(cells['director2'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['director2_role_URI'].value + '">' + cells['director2_role'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['director3'].value), '', '<name'+ if(isBlank(cells['director3_URI'].value), '', ' valueURI="' + cells['director3_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['director3'].value + '</namePart>' + if(isBlank(cells['director3'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['role2_URI'].value + '">' + cells['role2'].value + '</roleTerm></role>') + '</name>')}}
{{if(isBlank(cells['director4'].value), '', '<name'+ if(isBlank(cells['director4_URI'].value), '', ' valueURI="' + cells['director4_URI'].value + '"' + ' authority="naf"') + '><namePart>' + cells['director4'].value + '</namePart>' + if(isBlank(cells['director4'].value), '', '<role><roleTerm authority="marcrelator" valueURI="' + cells['role2_URI'].value + '">' + cells['role2'].value + '</roleTerm></role>') + '</name>')}}
<physicalDescription><form authority="aat" valueURI="{{cells['form_URI'].value}}>{{cells['form'].value}}</form><


</mods>

```

## Row Separator

**LEAVE BLANK**

## Suffix

```
</modsCollection>
```