Run the pipeline for multiple clients in sequence. Process each one completely before moving to the next.

Ask the user to provide a list of clients. For each client, they need:
1. Client name
2. Their business (what they do)
3. Their offer (what they sell, price point)
4. Target audience (who they serve)
5. Website URL
6. What they need produced (deliverables list)

Then process each client sequentially:
1. Run full pipeline (Research + Auto-Route + Execute) for Client 1
2. Save all deliverables to deliverables/[client-name]/
3. Save client context to memory/clients/[client-name].md
4. Run the per-client quality gate from CLAUDE.md
5. Announce completion and transition to next client
6. Repeat for each client

Follow the BATCH QUALITY ENFORCEMENT and Anti-Degradation Rules from CLAUDE.md. Every client gets fresh research, fresh copy, and fresh quality checks. Never reuse copy between clients.
