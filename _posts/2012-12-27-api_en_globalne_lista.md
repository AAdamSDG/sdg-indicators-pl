---
title: 'Download titles for global indicators'
type: 'GET'
name: '/api/en/globalne/lista.json'
lang: 'en'
---

This method allows users to download titles for all global indicators in English.

### Parameters

<p>No input parameters</p>

<p style='float:left;margin-top: 7px;'>Response content type</p>
<select style='float:left;padding: 0px 15px;width: 155px;margin-left: 10px;text-align-last: center;'>
  <option>application/json</option>
</select>

<div id='example'>

<h3 id="przykładowy-curl">Curl example</h3>

<p><code class="highlighter-rouge">curl -X GET --header 'Accept: application/json' 'https://api.github.com/repos/statisticspoland/sdg-indicators-pl/contents/api/en/globalne/lista.json'</code></p>

<h3 id="przykładowy-url">URL example</h3>

<p><code class="highlighter-rouge">https://api.github.com/repos/statisticspoland/sdg-indicators-pl/contents/api/en/globalne/lista.json</code></p>

<h3 id="przykładowy-kod-odpowiedzi">Response code</h3>

<p><code class="highlighter-rouge">200</code></p>

<h3 id="przykładowa-odpowiedź">Response</h3>

<p><code class="highlighter-rouge" id="show-data-glob-lista-en">
</code></p>

</div>


<script>

$.getJSON('https://sdg.gov.pl/api/en/globalne/lista.json', function(data) {
    $('#show-data-glob-lista-en').html(JSON.stringify(data, null, 2));
});

</script>
