```md
# Minecraft Server Log Field Extraction

- Extracted player IP addresses using regex:

```regex
^(?:[^\[\n]*\[){3}/(?P<Player_IP>[^:]+)
Used Splunk Field Extractor for validation

Fields can be used in searches and dashboards
