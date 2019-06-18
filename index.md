# License Zero Jurisdictions

[licensezero.com](https://licensezero.com) and the License Zero [command-line interface](https://guide.licensezero.com/#command-line-interface) use [ISO 3166-2 codes](https://en.wikipedia.org/wiki/ISO_3166-2) to identify the jurisdictions, or legal homes, or developers and customers.

Jurisdiction codes help to identify individuals with common names, and give developers and customers information they may need to comply with tax or other compliance requirements.

## Supported Jurisdictions

The list of ISO 3166-2 codes for jurisdictions that License Zero supports is also available as [an npm package](https://www.npmjs.com/package/licensezero-jurisdictions).

<ul style="columns: 6;">
{% assign jurisdictions = site.data.jurisdictions | sort %}
{% for code in jurisdictions %}
<li><a href="https://www.iso.org/obp/ui/#iso:code:3166:{{ code | slice: 0, 2 }}">{{code}}</a></li>
{% endfor %}
</ul>
