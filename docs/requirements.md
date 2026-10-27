Requirement 1 — How the ticket works
Our current design is:
1. A passenger has a transport card with a wallet balance.
2. The passenger purchases a ticket using that balance.
3. The ticket remains purchased but inactive until the first successful validation.
4. At the first successful validation, the ticket activates for 120 minutes.
5. During those 120 minutes, eligible journeys should not cause another ticket charge.
6. Once the ticket expires, the passenger must purchase another ticket.
The server manages the authoritative wallet balance and transaction history. The Java Card simulator will let us develop and test card-side behavior before using physical smart cards.



