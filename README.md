# DAA-Project-Algorithm-Binary-Search-Student-Record-Sorting
A browser-based DAA project for managing student records and visualizing sorting and searching algorithms. Compare algorithm performance, explore time and space complexity, and manage records with a simple responsive interface.
Student Name: Jenil Patel
Enrollment Number: 12402080601053
Department / Division: Information Technology (IT-A)
Semester: V
**Link To test the Project:**C:/Users/patel/Documents/Codex/2026-10-21/https-github-com-vishrut2105-daa-project/outputs/index.html
# CampusIndex — Student Record Sorting & Searching System.

A browser-based Design and Analysis of Algorithms project for managing student records and learning how classic sorting and searching algorithms work. It uses HTML, CSS, and dependency-free JavaScript. Student data is stored in the browser with `localStorage`.

## Features

- Add, edit, delete, filter, and sort student records.
- Export records to CSV; restore the original sample dataset at any time.
- Visualize Bubble, Selection, Insertion, Merge, Quick, and Heap Sort on records keyed by marks, CGPA, name, or student ID.
- Compare all six sorting algorithms on the same input with comparison counts, writes, elapsed time, and complexity.
- Trace Linear Search and Binary Search for a selected student ID.
- Review best, average, and worst time complexity, auxiliary space, and sorting stability.
- Responsive dashboard with summary statistics and recent student records.

## Run it

Open `index.html` in a modern browser. No installation or build step is required. Alternatively, run a local server from this directory:

```sh
python -m http.server 8080
```

Then visit `http://localhost:8080`.

## Project files

```text
outputs/
├── index.html       # App views and dialogs
├── styles.css       # Responsive dashboard and visualization styling
├── README.md        # Project overview and run instructions
└── js/
    └── app.js       # Records, algorithms, visualization, and navigation
```

## Algorithm summary

| Algorithm | Best | Average | Worst | Auxiliary space | Stable |
|---|---:|---:|---:|---:|:---:|
| Bubble Sort | Ω(n) | Θ(n²) | O(n²) | O(1) | Yes |
| Selection Sort | Ω(n²) | Θ(n²) | O(n²) | O(1) | No |
| Insertion Sort | Ω(n) | Θ(n²) | O(n²) | O(1) | Yes |
| Merge Sort | Ω(n log n) | Θ(n log n) | O(n log n) | O(n) | Yes |
| Quick Sort | Ω(n log n) | Θ(n log n) | O(n²) | O(log n) average | No |
| Heap Sort | Ω(n log n) | Θ(n log n) | O(n log n) | O(1) | No |
| Linear Search | Ω(1) | Θ(n) | O(n) | O(1) | — |
| Binary Search | Ω(1) | Θ(log n) | O(log n) | O(1) | — |

Binary Search sorts the student IDs before searching, so its displayed count measures the search phase. Benchmark timings are browser and device dependent; comparison and write counts are more repeatable.

## Suggested DAA project explanation

The project models each student as a record and applies sorting and searching based on selected fields. It demonstrates the difference between quadratic and n-log-n sorting behavior, and between sequential and logarithmic search on ordered IDs. The benchmark provides empirical counts and timings while the complexity guide summarizes theoretical growth. Data is kept in the current browser profile and is not uploaded to a server.
