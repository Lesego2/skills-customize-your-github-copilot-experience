# Project Description

This project is an educational website for sharing homework assignments and coding exercises with students. Students can browse, view, and download assignments directly from the portal.

## Project Structure

- [`assignments/`](../assignments/) Each homework assignment is stored in its own subfolder with a consistent structure.
- [`templates/`](../templates/) Reusable templates for new content
- [`assets/`](../assets/) Contains the website assets including CSS, JavaScript, images, and configuration files
- [`index.html`](../index.html) The main website page that serves as a static portal for browsing and viewing assignments. Content is driven by [`config.json`](../config.json), a build-time configuration file that must conform to the provided JSON schema at [`config.schema.json`](../config.schema.json). `config.json` must contain an array `assignments` with fields: `id`, `title`, `difficulty`, `tags`, `path`, and `publishDate`. The static build process should validate `config.json` against `config.schema.json`; if the file is missing, malformed, or fails schema validation, the build must abort with a human-readable error message listing the invalid fields. At runtime, if the loaded configuration is invalid, display "Configuration error — contact instructor" and render a minimal default index with no assignments.

## Project Guidelines

- Maintain consistent styling across all pages
- Keep file and folder names descriptive and organized
 - Keep file and folder names descriptive and organized. Use the following naming conventions to avoid ambiguity:
	 - Use kebab-case (lowercase words separated by single dashes), e.g. `intro-to-loops`.
	 - No spaces or special characters; only lowercase letters, numbers, and dashes are allowed.
	 - Prefix assignment folders with a zero-padded numeric id, e.g. `01-intro-to-loops`, `02-variables-and-types`.
	 - Limit names to 60 characters.

## Educational Standards

When generating content for this project:

- **Learning-focused**: All content should be designed with clear learning objectives and appropriate difficulty levels
- **Student-friendly**: Use clear, encouraging language that motivates students