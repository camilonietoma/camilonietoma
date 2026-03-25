---
layout: page
title: data
permalink: /data/
nav: true
nav_order: 4
---

<style>
.rep-header { padding: 1rem 0; border-bottom: 0.5px solid #e0e0e0; margin-bottom: 1.5rem; }
.rep-card { background: #fff; border: 0.5px solid #e0e0e0; border-radius: 12px; padding: 1rem 1.25rem; margin-bottom: 0.75rem; display: flex; align-items: center; justify-content: space-between; gap: 1rem; }
.rep-card:hover { border-color: #bbb; }
.rep-title { font-size: 14px; font-weight: 500; margin: 0 0 4px; line-height: 1.4; }
.rep-journal { font-size: 12px; color: #888; margin: 0; }
.rep-link { display: inline-flex; align-items: center; gap: 5px; font-size: 12px; font-weight: 500; color: #185FA5; background: #E6F1FB; border: 0.5px solid #85B7EB; border-radius: 8px; padding: 5px 10px; white-space: nowrap; text-decoration: none; flex-shrink: 0; }
.rep-link:hover { opacity: 0.85; }
.rep-hidden { display: none; }
.rep-toggle { width: 100%; margin-top: 0.5rem; padding: 8px; font-size: 13px; cursor: pointer; background: transparent; border: 0.5px solid #ccc; border-radius: 8px; color: #555; }
.rep-toggle:hover { background: #f5f5f5; }
</style>

<div class="rep-header">
  <p style="font-size: 13px; color: #888; margin: 0;">Replication data and materials for published research. Files are hosted on GitHub.</p>
</div>

<div class="rep-card">
  <div>
    <p class="rep-title">The Violent Path to Power: Violence Against Social Activism and the Rise of Criminal Politicians</p>
    <p class="rep-journal">Journal of Politics in Latin America, 2025</p>
  </div>
  <a class="rep-link" href="LINK_1">&#8594; Data</a>
</div>

<div class="rep-card">
  <div>
    <p class="rep-title">State Violence and the Political Consequences of Property Rights: Evidence from Colombia</p>
    <p class="rep-journal">Studies in Comparative International Development, 2025</p>
  </div>
  <a class="rep-link" href="LINK_2">&#8594; Data</a>
</div>

<div class="rep-card">
  <div>
    <p class="rep-title">Spraying Conflict: Aerial Drug Eradication and Armed Violence in Colombia</p>
    <p class="rep-journal">British Journal of Political Science, 2025</p>
  </div>
  <a class="rep-link" href="LINK_3">&#8594; Data</a>
</div>

<div class="rep-card">
  <div>
    <p class="rep-title">Mining and Violence in Latin America: The State's Coercive Responses to Anti-Mining Resistance</p>
    <p class="rep-journal">World Development, 2024</p>
  </div>
  <a class="rep-link" href="LINK_4">&#8594; Data</a>
</div>

<div class="rep-card">
  <div>
    <p class="rep-title">Why Programmatic Parties Reduce Criminal Violence: Theory and Evidence from Brazil</p>
    <p class="rep-journal">Research & Politics, 2023</p>
  </div>
  <a class="rep-link" href="LINK_5">&#8594; Data</a>
</div>

<div class="rep-card rep-hidden" id="extra-1">
  <div>
    <p class="rep-title">When the State Becomes Complicit: Mayors, Criminal Actors, and the Deliberate Weakening of the Local State in Colombia</p>
    <p class="rep-journal">Comparative Political Studies, 2023</p>
  </div>
  <a class="rep-link" href="LINK_6">&#8594; Data</a>
</div>

<div class="rep-card rep-hidden" id="extra-2">
  <div>
    <p class="rep-title">Containing Large-Scale Criminal Violence Through Internationalized Prosecution</p>
    <p class="rep-journal">Comparative Political Studies, 2023</p>
  </div>
  <a class="rep-link" href="LINK_7">&#8594; Data</a>
</div>

<div class="rep-card rep-hidden" id="extra-3">
  <div>
    <p class="rep-title">Land and State Capacity During Civil Wars: How Land-Based Coalitions Undermine Property Taxation in Colombia</p>
    <p class="rep-journal">Journal of Conflict Resolution, 2023</p>
  </div>
  <a class="rep-link" href="LINK_8">&#8594; Data</a>
</div>

<div class="rep-card rep-hidden" id="extra-4">
  <div>
    <p class="rep-title">Democracy in the Countryside: The Rural Sources of Violence against Voters in Colombia</p>
    <p class="rep-journal">Journal of Peace Research, 2019</p>
  </div>
  <a class="rep-link" href="LINK_9">&#8594; Data</a>
</div>

<button class="rep-toggle" id="toggle-btn" onclick="toggleMore()">Show more</button>

<script>
function toggleMore() {
  var extras = document.querySelectorAll('[id^="extra-"]');
  var btn = document.getElementById('toggle-btn');
  var hidden = extras[0].classList.contains('rep-hidden');
  extras.forEach(function(el) { el.classList.toggle('rep-hidden', !hidden); });
  btn.textContent = hidden ? 'Show less' : 'Show more';
}
</script>
