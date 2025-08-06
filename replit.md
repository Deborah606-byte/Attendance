# Overview

This is a mobile-first attendance tracking application built with React, TypeScript, and Express.js. The app allows users to track attendance with location services, manage work site information, and view attendance history. It features a modern UI using shadcn/ui components and Tailwind CSS, with a focus on mobile user experience.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **React 18** with TypeScript for type safety
- **Vite** as the build tool and development server
- **Wouter** for lightweight client-side routing
- **shadcn/ui** component library with Radix UI primitives
- **Tailwind CSS** for styling with CSS variables for theming
- **TanStack React Query** for server state management and API caching
- **React Hook Form** with Zod validation for form handling

## Backend Architecture
- **Express.js** server with TypeScript
- **RESTful API** design pattern (routes prefixed with `/api`)
- **In-memory storage** implementation with interface for easy database migration
- **Session-based architecture** with middleware for request logging
- **Modular route registration** system

## Data Layer
- **Drizzle ORM** configured for PostgreSQL with Neon Database
- **Database migrations** managed through Drizzle Kit
- **Zod schemas** for runtime validation and type inference
- **Shared schema** between client and server for type consistency

## UI/UX Design
- **Mobile-first** responsive design approach
- **Dark/light theme** support with CSS custom properties
- **Component-driven** architecture with reusable UI primitives
- **Accessibility-focused** components using Radix UI
- **Toast notifications** for user feedback

## Development Setup
- **ESM modules** throughout the application
- **Path aliases** for clean imports (@/, @shared/, @assets/)
- **TypeScript strict mode** enabled for better code quality
- **Hot module replacement** in development with Vite
- **Error overlay** integration for development debugging

# External Dependencies

## Database & ORM
- **Neon Database** - Serverless PostgreSQL database
- **Drizzle ORM** - Type-safe SQL toolkit and query builder
- **connect-pg-simple** - PostgreSQL session store for Express

## UI Framework & Styling
- **Radix UI** - Headless UI components for accessibility
- **Tailwind CSS** - Utility-first CSS framework
- **Lucide React** - Icon library
- **class-variance-authority** - Utility for creating variant-based component APIs

## Development Tools
- **Replit integration** - Development environment optimizations
- **esbuild** - Fast JavaScript bundler for production builds
- **PostCSS** - CSS post-processing with Autoprefixer

## Third-party Services
- **Location Services** - Browser geolocation API for attendance tracking
- **Camera API** - Web camera access for photo capture functionality

## Additional Features
- **Date manipulation** using date-fns library
- **Carousel components** with Embla Carousel
- **Command palette** functionality with cmdk