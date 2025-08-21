# Overview

This is a full-stack web application built as a U.S. Bank customer service portal mockup. The application provides a comprehensive customer service interface with search functionality, popular topics, service areas, and contact information. It's built using modern web technologies with a React frontend and Express backend, designed to demonstrate a professional banking customer service experience.

The application features a clean, responsive design that mirrors professional banking websites, with sections for searching customer service topics, browsing popular banking tasks, exploring different service areas, and accessing contact information.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety and modern component patterns
- **Routing**: Wouter for lightweight client-side routing
- **UI Components**: shadcn/ui component library built on Radix UI primitives for accessible, customizable components
- **Styling**: Tailwind CSS with custom design system variables for consistent theming
- **State Management**: TanStack Query (React Query) for server state management and caching
- **Build Tool**: Vite for fast development and optimized production builds

## Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules for modern JavaScript features
- **Development Setup**: Hot reload with Vite integration for seamless full-stack development
- **Storage Layer**: Abstracted storage interface with in-memory implementation (MemStorage class)
- **API Design**: RESTful API structure with `/api` prefix routing

## Database Layer
- **ORM**: Drizzle ORM for type-safe database operations
- **Database**: PostgreSQL configured via Drizzle with Neon serverless driver
- **Schema Management**: Centralized schema definitions in shared directory with Zod validation
- **Migrations**: Drizzle Kit for database schema migrations

## Development Workflow
- **Monorepo Structure**: Client and server code in separate directories with shared schema
- **Path Aliases**: TypeScript path mapping for clean imports (@/, @shared/, @assets/)
- **Development Server**: Integrated Vite dev server with Express middleware mode
- **Hot Reload**: Full-stack hot reload during development

## Design System
- **Component Library**: Custom implementation using shadcn/ui patterns
- **Theme System**: CSS custom properties with light/dark mode support
- **Typography**: Inter font family with multiple weight variations
- **Color Palette**: Custom U.S. Bank brand colors integrated into Tailwind config
- **Responsive Design**: Mobile-first approach with consistent breakpoints

# External Dependencies

## Database Services
- **Neon Database**: Serverless PostgreSQL hosting with connection pooling
- **PostgreSQL**: Primary database engine for persistent data storage

## UI Component Libraries
- **Radix UI**: Comprehensive set of accessible, unstyled UI primitives
- **Lucide React**: Icon library providing consistent iconography
- **Embla Carousel**: Touch-friendly carousel component for content display

## Development Tools
- **Vite**: Build tool and development server with plugin ecosystem
- **ESBuild**: Fast bundling for production builds
- **PostCSS**: CSS processing with Tailwind CSS integration

## Styling and Design
- **Tailwind CSS**: Utility-first CSS framework with custom configuration
- **Class Variance Authority**: Type-safe variant management for component styling
- **clsx**: Utility for conditional CSS class composition

## Form and Validation
- **React Hook Form**: Performant forms with easy validation
- **Zod**: TypeScript-first schema validation library
- **Hookform Resolvers**: Integration between React Hook Form and Zod

## Utility Libraries
- **date-fns**: Modern date utility library for date formatting and manipulation
- **nanoid**: URL-safe unique string ID generator

## Development Environment
- **Replit Integration**: Custom plugins for Replit development environment
- **TypeScript**: Type checking and enhanced developer experience
- **Node.js**: JavaScript runtime for server-side execution