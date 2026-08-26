# FurEver Care - Short Project Report

## 1. Problem Definition
Pet owners often manage feeding, grooming, health information, product discovery and appointments across different sources. Shelters need a clear way to showcase adoptable pets, while veterinarians need organized views of profiles, time slots and example medical histories. FurEver Care centralizes these front-end experiences into one responsive single-page portal.

## 2. Design Specifications
- SPA navigation with role-specific menus.
- Responsive mobile-first layout using Bootstrap utilities plus custom CSS.
- Colorful pet-friendly visual language with violet, pink, mint, orange and cyan accents.
- Accessible forms, clear labels, keyboard-friendly buttons and visible focus states.
- Static data files only; no server-side data storage.

## 3. Flowchart
```text
Start
  |
Enter first name + choose role
  |--------------------|---------------------|
Pet Owner              Veterinarian          Shelter
  |                     |                    |
Pet profile form        Vet profile form     Adoption gallery
  |                     |                    |
Owner dashboard         Vet dashboard        Stories / Events / Contact
  |
Care / Products / Emergency / Feedback / Contact
```

## 4. Data Flow Summary
```text
JSON files --------> JavaScript fetch ------> Product / Adoption / Case Study UI
XML files ---------> jQuery AJAX -----------> Emergency / Event UI
TXT file ----------> Fetch -----------------> Scrolling ticker
User forms --------> Browser session state -> Personalized dashboard
Geolocation API ---> JavaScript ------------> Location display
Clock -------------> JavaScript ------------> Real-time display
```

## 5. Test Data
- Owner: Ali / Dog / Max / Labrador / 3 years / Up to date
- Vet: Dr. Sara / Small Animal Medicine / doctor@example.com / +92 300 0000000
- Shelter filter examples: Dog, Cat, Rabbit; Young, Adult, Senior; Karachi search
- Product search examples: food, toy, grooming; sort by price and name

## 6. Installation
Run through VS Code Live Server or `python -m http.server 8000`, then open `http://localhost:8000`.

## 7. Assumptions
- No back-end is required or used.
- Buy Now and appointment slots are display-only as specified.
- Demo contact numbers are fictional/static.
- Product prices are illustrative PKR values.
- External images/maps/video require internet access; local UI still works with image fallbacks.

## 8. Diagrams
- `docs/flowchart.svg` - role-based user flow.
- `docs/data-flow-diagram.svg` - front-end data flow for forms, browser APIs, JSON, XML and TXT.

## 9. Requirement Traceability
See `SRS_COMPLIANCE.md` for a feature-by-feature implementation checklist.

## 10. Demonstration
A short visual walkthrough clip is included as `docs/FurEverCare_demo.mp4`.
