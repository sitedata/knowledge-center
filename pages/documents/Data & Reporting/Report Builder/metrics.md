---
pagename: Metrics
categoryName: Reporting & Data
subCategoryName: Report Builder
indicator: both
subtitle: " A comprehensive search of all the Metrics related to the Report Builder"
level3: ''
permalink: Reporting-&-data-report-builder-metrics
isTutorial: false
date: 2019-01-09 12:53:18 +0000

---
The table below outlines all of the data metrics available in the Report Builder, with their definition and location within the different dashboards. More information on the Report Builder can be found [here](https://knowledge.liveperson.com/data-reporting-report-builder-report-builder-overview.html).

<div id="metrics">
<input id="metricsSearch" placeholder="Search by Metric or Dashboard" />
<table class="metricstable" id="datametricstable">
  <thead>
    <tr>
      <th>Metric</th>
      <th class="analysis">Analysis Type</th>
      <th class="channel">Channel</th>
      <th class="description">Description</th>
      <th class="dashboard">Dashboard</th>
      <th class="filtered">Filtered By</th>
      <th class="formula">Formula (Optional)</th>
    </tr>
  </thead>
  <tbody class="list">
  {% for metricitem in site.data.reportbuilder %}
    <tr>
      <td class="metric">{{ metricitem.Metric }}</td>
      <td class="analysis">{{ metricitem.analysisType }}</td>
      <td class="channel">{{ metricitem.Channel }}</td>
      <td class="description">{{ metricitem.Description }}</td>
      <td class="dashboard">{{ metricitem.Dashboard }}</td>
      <td class="filtered">{{ metricitem.filteredBy }}</td>
      <td class="formula">{{ metricitem.formulaOptional }}</td>
    </tr>
  {% endfor %}
</tbody>
</table>
</div>
