# near-event-discovery

Daily experimental event discovery exports for Near.

This repo stores CSV snapshots generated from public Lima event sources while we
evaluate which sources are reliable enough to feed Near markers.

## Workflow

1. Search candidate event sources for Lima.
2. Normalize candidates into a dated CSV under `csv/`.
3. Commit and push the CSV.
4. Send a WhatsApp summary with a link to the CSV.
5. Do not create Near backend seeds or marker PRs until the sources are reviewed.

## CSV Format

```csv
date_found,event_title,event_date,start_time,end_time,venue,district,address,category,source_name,source_url,confidence_score,notes
```

## Candidate Sources

- EntradaLibre
- Heptagrama agenda cultural
- Teleticket
- Meetup Lima
- BNP eventos
- Songkick
- Bandsintown

## Naming

Daily CSV files use:

```text
csv/YYYY-MM-DD-lima-events.csv
```
