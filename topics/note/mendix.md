# Mendix

## Mendix Certification & Background (Chứng chỉ & Kiến thức nền)

**Q: Do you have any experience or certification in Mendix?**

* **Answer:** Yes. I have a Mendix Rapid Developer certificate. I understand the core concepts of Mendix, such as Domain Model, Microflows.

## Mendix vs Traditional Coding

**Q: Why should we use Mendix instead of traditional code (like Java, C#, React)?**

* **Answer:** Mendix helps us develop applications faster. It reduces the amount of code we need to write and makes it easier to work with business teams. For complex or special tasks, traditional coding can still be a better choice.

**Q: Is Low-code/Mendix replacing traditional developers?**

* **Answer:** No, it doesn't replace them. Mendix is a tool to boost productivity. Good Mendix developers still need strong traditional concepts like Database design, Security, APIs and System Architecture.

## Naming Conventions (Quy tắc đặt tên)

**Q: How to name Microflows and Nanoflows in Mendix?**

* **Answer:** We name Microflows and Nanoflows using the formula: `[Prefix]_[Entity]_[Action]`. For example, `ACT_Customer_Save` for a save button action.
* **Notes:**
  * Use PascalCase for the Entity and Action names.
  * Common Prefixes to remember:
    * `ACT_`: Action triggered by a button / click
    * `SUB_`: Sub-microflow called inside another microflow.
    * `VAL_`: Validation microflow.
    * `Och_`: On-Change event handler.

**Q: How to name Domain Model?**

* **Answer:** Entities and Attributes use PascalCase without prefixes. Entites must be sigular nouns. Associations use the formula: `[ParentEntity]_[ChildrenEntity]`

**Q: How to name Pages in Mendix?**

* **Answer:** We name Pages using PascalCase with the formula `[Entity]_[PageType]`. For example, `Customer_Overview`
* **Notes:**
  * `_Overview`: List/grid page showing multiple records.
  * `_NewEdit`: Form page to create or update a record.
  * `_Detail`: View-only page for details.

## Core Technical Concepts (Kiến thức kỹ thuật Mendix)

**Q: What is a Domain Model in Mendix and how do you use it?**

* **Answer:** A Domain Model is the data structure of the application. It contains Entities and Attributes to store data, and Associations to connect different entities together.

**Q: What is the difference between a Microflow and a Nanoflow?**

* **Answer:** Microflows run on the server side to handle complex business logic and database operations. Nanoflows run on the client side (in the browser or mobile app), so they run faster and can work offline.
* **Notes:**
  * Microflow: Server-side
  * Nanoflow: Client-side

**Q: How do you handle security in Mendix?**

* **Answer:** Mendix provides security at two levels: Module Level and Project Level. First, I define Module Roles for specific features, and then map them to User Roles at the Project Level, like Admin, Manager or Customer.
* **Notes:**
  * We separate Project Roles and Module Roles for reusability.
  * A module has its own roles and security rules.
  * When we use the same module in another project, we can map its Module Roles to the new Project Roles.
  * This means we do not need to setup the module security again from the beginning.

## Financial Domain Application (Ứng dụng Mendix trong dự án Tài chính)
