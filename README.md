![Maui](assets/maui.webp)

# Problem

Maui was asked by the gods to guard Apulalula Island and grant access to important places only for those worthy. Maui excels at combat but struggles with memory, especially regarding who is allowed to enter specific locations.

**Your mission: Help Maui manage access control with a robust full-stack tool.**

## Maui's Requirements for the Tool

1. Maintain records of all places (can be hardcoded).
2. Citizens have roles granting access to specific places (citizens and roles can be hardcoded).
3. Roles can have sub-roles, inheriting permissions.
4. Maui will use the tool to verify citizen access, so a user-friendly UI is essential.
5. **Record every access check (allowed or denied) in the system and provide a UI to review access logs.**

## Your Task

Create a full-stack web application with both frontend and backend components, storing data in a database of your choice (MongoDB preferred, but you may choose any suitable database).

## Technical Requirements

### Frontend
- Develop an intuitive UI using React (preferred) or another modern framework.
- UI must include:
  - Form with dropdown fields to select citizens and places.
  - Upon submission, validate access via backend and clearly indicate approval or denial.
  - **Separate page or component displaying an access logs table, showing citizen, place, result (allowed/denied), and timestamp.**

Screens should look something like that:

![form](assets/access-form.png)

![submission-success](assets/access-approved.png)

![submission-failure](assets/access-denied.png)

![logs](assets/access-log.png)


### Backend
- RESTful API with any preferred technology stack (Node.js with NestJS preferred, but you may use any stack you're comfortable with).
- Implement data models for:
   - Citizens (name, roles)
   - Roles (name, subRoles)
   - Places (name, rolesAllowed)
   - Access logs (citizen + role, place, access result, timestamp)
- Tests covering critical business logic
- **Role hierarchy (parent-child roles)**

### Database
- Database of your choice (MongoDB preferred)
- Schema supporting:
  - Access logs (citizen, place, timestamp, result)

## Functional Requirements
- Quickly validate citizen access to a place
- Record each access attempt (success or failure)
- Provide UI to review detailed access logs

## Bonus Points
- Proper error handling and input validation
- Unit tests covering critical business logic (required)
- **Dynamic management of citizens, roles, and places via additional API endpoints (UI optional).**

## Submission Requirements
- Pull request to the repository
- API documentation (optional)
- Explanation of technical decisions and architecture
- List of assumptions made

## Evaluation Criteria
- Code quality and architecture
- Type safety and error handling
- Performance and scalability considerations
- Security best practices
- Testing coverage
- Documentation clarity
- Implementation of logging requirements

## Time Estimate
This assignment should take approximately **5-6 hours** to complete. Submit your solution within **5 days**.
