SHUBHVASTRA — User Permission Update

Member
- Dashboard અને Party Master view; Party Master માં નવી Party ઉમેરવાની પરવાનગી.
- New Order બનાવી શકે, પરંતુ existing Order edit કરી શકતો નથી.
- Item Master માં SKU add કરી શકે; SKU edit ફક્ત Admin.
- Agent Master માં Agent add કરી શકે; Agent edit ફક્ત Admin.
- Pending to Dispatch Order દ્વારા dispatch/cancel workflow કરી શકે.
- Dispatched Details અને Order Reports જોઈ શકે.
- Order History / Order List view અને PDF download; Edit/Delete controls ફક્ત Admin માટે.
- Admin Panel અને Backup/Restore access નથી.
- Party Edit અને Party Excel Import/Export access નથી.

Staff
- Dashboard માં ફક્ત Party Name અને City.
- New Order, Party Master, Item Master, Agent Master, Order History, Cancelled Orders અને Order Reports access નથી.
- Pending to Dispatched menu માં ફક્ત Party Wise Pending Report, Agent Wise Pending Report અને SKU Wise Pending Report; ત્રણેય PDF download કરી શકે.
- Pending to Dispatch Order screen અને dispatch/cancel action access નથી.
- Dispatched Details view-only; કોઈ edit/cancel action નથી.
- Admin Panel access નથી.

Agent
- અગાઉની Agent role ની own-agent party scoping અને read-only portal જાળવેલ છે.

Admin
- Existing full admin access યથાવત્.

Deployment:
- GitHub માં આ update ના code files upload કરો.
- Existing database file / DATABASE_URL ને delete કે replace ન કરશો.
- Deploy પછી દરેક role થી અલગ login કરીને permissions test કરશો.
