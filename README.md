# Tugas-Tailwind-P2
Muhammad Rio(2411102441270)

Penjelasan Desain
1. Mobile-First Approach
Desain dimulai dari tampilan mobile (320px) kemudian dikembangkan untuk tablet dan desktop menggunakan breakpoint Tailwind:

Default (mobile): Layout vertikal, grid 1 kolom
md (768px+): Layout horizontal, grid 3 kolom
lg (1024px+): Layout expanded, grid 4 kolom

2. Fitur Tailwind yang Digunakan
   
a. Responsive Utilities

grid-cols-1 md:grid-cols-3 lg:grid-cols-4 - Grid responsif
flex-col md:flex-row - Layout direction yang berubah
text-center md:text-left - Text alignment responsif
justify-center md:justify-start - Justify content responsif

b) Order & Layout Control

order-1 md:order-1 - Profile picture order
order-2 md:order-3 - Button positioning
order-3 md:order-2 - Content reordering

c) Grid Spanning & Nesting

md:col-span-2 lg:col-span-2 - Featured post spanning
md:col-span-1 lg:col-span-2 - Dynamic column spanning
Nested grid dalam card untuk layout yang lebih kompleks

3. Component Breakdown
Header Profil

Sticky navigation dengan sticky top-0 z-50
Responsive icon visibility dengan hidden md:block

Profile Section

Flexbox dengan responsive direction
Profile picture dengan gradient border custom
Stats dengan spacing yang konsisten
Action buttons yang berubah layout di berbagai breakpoint

Story Highlights

Horizontal scroll dengan overflow-x-auto
Consistent sizing dengan flex-shrink-0

Photo Feed

Advanced grid layout dengan spanning
Hover effects dengan group dan group-hover:
Image overlay dengan opacity transitions
Nested grids untuk variasi visual

Tantangan Layout yang Diselesaikan
1. Complex Grid Layout

Menggunakan col-span untuk featured posts
Nested grids untuk variasi visual
Responsive spanning yang berbeda per breakpoint

2. Flexible Component Ordering

Profile elements yang reorder pada tablet/desktop
Button positioning yang optimal untuk setiap device
Content hierarchy yang logical

3. Interactive States

Hover effects pada feed posts
Button state management
Smooth transitions dan transformations

📱 Responsive Behavior
Mobile (< 768px)

Single column grid
Vertical profile layout
Full-width buttons
Bottom navigation
Optimized touch targets

Tablet (768px - 1024px)

3-column feed grid
Horizontal profile layout
Balanced button sizes
Hidden mobile navigation

Desktop (1024px+)

4-column feed grid
Expanded profile section
Larger interactive elements
Enhanced hover states

Pertanyaan Reflektif
1. Mengapa memilih Mobile-First Approach?
Mobile-first memastikan core functionality bekerja pada device dengan constraint terbesar (layar kecil, bandwidth terbatas). Ini mendorong prioritisasi content dan progressive enhancement untuk device yang lebih capable.
2. Bagaimana Tailwind CSS mempengaruhi workflow development?
Positif:

Rapid prototyping dengan utility classes
Consistent design system built-in
Reduced CSS file size dengan unused class purging
Inline styling yang readable dan maintainable
