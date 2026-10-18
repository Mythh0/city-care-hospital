# CityCare Hospital Triage System (demo)

Open `index.html` in any browser. No install or server needed.

## Interfaces
- Patient: check in with validation, get a Patient ID, see the reason for the assigned priority, track queue position.
- Admin (password: 1234): dashboard, register patients, searchable and filterable queue with priority reasons, history, reports (printable), DSA view.

## Data structures
- Max-Heap (Emergency and Serious): insert / extractMax in O(log n). Highest priority is served first, ties go to the earliest arrival.
- Queue, FIFO (Normal): enqueue / dequeue in O(1).
- Treat next patient calls extractMax() on the heap first, and dequeue() on the queue only when the heap is empty.

## Notes
- Demonstration only. All patients are fictional. The priority rules are simple teaching examples and have not been reviewed by medical professionals. Any real clinical prioritisation must be reviewed and approved by qualified clinicians.
- Data is saved in the browser (localStorage). "Reset demo data" on the admin dashboard regenerates random patients.
- Fonts load from Google Fonts and fall back to system fonts when offline.
