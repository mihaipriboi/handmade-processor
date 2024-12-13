## Key Decisions Made and Their Reasoning

### Structure Overview
Each entry includes:
1. **Date** – When the decision was made.
2. **Decision** – A clear statement of the choice.
3. **Reasoning** – Why this choice was made, including any alternatives considered.
4. **Impact** – What this decision affects or changes in the project.
5. **Revisions** (optional) – Updates to this decision later, if applicable.

### Entries

#### [2024-12-13]
**Decision:** Use **breadboards** instead of prototype boards for the first hardware assembly prototype.

**Reasoning:**
- Provides flexibility for testing and prototyping.
- Facilitates quick modifications and component replacements.
- Faster to assemble and disassemble for iterative development.
- Allows hands-on assembly without relying on outsourced PCBs.
- Fits the project’s goal of being a personal, handmade effort.

**Impact:**
- Makes the initial hardware bigger and less compact.
- Will require a detailed wiring plan and efficient use of space.
- May face challenges with component stability due to the nature of breadboarding.

---

**Decision:** Visual identity color chosen for the project: <span style="color:#702963;"><strong>Byzantium</strong></span> (`#702963`).

**Reasoning:**
- Byzantium is a rich, deep color that conveys creativity and ambition.
- The shade is distinctive and memorable, setting the project apart.

**Impact:**
- Will be used in project branding, visuals, and design elements.
- Provides a consistent color theme across project materials.
- Ensures visual cohesiveness in the project's aesthetic.

---

**Decision:** The processor will use a **16-bit data bus** and a **16-bit address bus**.

**Reasoning:**
- A 16-bit data bus allows the processor to handle 16 bits of data in one operation, which is a reasonable choice for this design's simplicity and ease of implementation.
- A 16-bit address bus enables the processor to address up to **64KB** of memory, which fits the project’s initial design goal.

**Impact:**
- Restricts the addressable memory to **64KB**.
- Limits the data width to **16 bits**, which is sufficient for handling basic operations, but may need expansion if future design goals require more data throughput.

---

**Decision:** The processor will have **64KB** of RAM, determined by the 16-bit address bus width.

**Reasoning:**
- The 16-bit address bus allows addressing a maximum of **64KB** of memory.
- This is a practical and standard choice for an initial design, offering enough space for basic programs while fitting the project's constraints.
- Although memory can be expanded using techniques like paging or bank switching, this size is sufficient for the current phase.

**Impact:**
- Requires efficient memory management.

---

**Decision:** The processor will have **8 general-purpose registers (R0 to R7)**, each 16 bits wide.

**Reasoning:**
- The **8 general-purpose registers** provide sufficient temporary storage for data during computation, supporting basic operations such as loading, storing, and manipulating data.
- Using **16-bit registers** matches the processor's **16-bit data bus** and allows for easier integration with other components, such as the **ALU** and **RAM**.
- These registers are necessary for storing intermediate results in basic programs.

**Impact:**
- Defines the internal data storage for the processor.
- Supports the simplicity and efficiency of the initial design.
- Ensures the processor has enough registers for basic operations, avoiding complexity and overhead with more than 8 registers at this stage.

---

**Decision:** Use **Logisim Evolution** for the processor design.

**Reasoning:**
- **Logisim Evolution** is a powerful and intuitive tool for designing and simulating digital circuits.
- It offers flexibility to build and test designs virtually before physical implementation, which is crucial for prototyping and debugging.
  
**Impact:**
- Simplifies the design and testing phase by allowing for easy visualization of the processor’s behavior.
- Reduces errors before hardware implementation, ensuring a smoother transition to breadboarding.

---
