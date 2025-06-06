# Mergington High School Activities

A comprehensive web application for managing extracurricular activities at Mergington High School. The system provides students with an intuitive interface to discover and explore activities, while offering teachers powerful tools to manage student registrations.

## Features

### Student Features
- **Browse Activities**: View all available extracurricular activities with detailed information
- **Advanced Search**: Search activities by name, description, or keywords
- **Smart Filtering**: Filter activities by:
  - Category (Sports, Arts, Academic, Community, Technology)
  - Day of the week (Monday through Sunday)
  - Time slot (Before School, After School, Weekend)
- **Activity Details**: View comprehensive information including:
  - Activity descriptions and schedules
  - Meeting days and times
  - Current enrollment and capacity limits
  - Participant lists

### Teacher Authentication & Management
- **Secure Login**: Teachers can log in with their credentials
- **Student Registration**: Register students for activities on their behalf
- **Student Management**: Unregister students from activities when needed
- **Real-time Updates**: Changes are reflected immediately in the interface

### Technical Features
- **Responsive Design**: Optimized for desktop and mobile devices
- **Real-time Filtering**: Instant search and filter results
- **Interactive UI**: Modal dialogs and smooth animations
- **RESTful API**: Clean API endpoints for all functionality
- **Data Persistence**: MongoDB database for reliable data storage

## Activity Categories

The system supports diverse extracurricular activities across multiple categories:

- **Sports**: Soccer Team, Basketball Team, Morning Fitness
- **Arts**: Art Club, Drama Club
- **Academic**: Chess Club, Math Club, Debate Team, Science Olympiad
- **Technology**: Programming Class, Weekend Robotics Workshop
- **Community**: Various community service and social activities
- **Special Interest**: Manga Maniacs and other student interest groups

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/activities` | Get all activities with optional filtering by day and time |
| GET | `/activities/days` | Get list of available activity days |
| POST | `/activities/{activity_name}/signup` | Register a student for an activity |
| POST | `/activities/{activity_name}/unregister` | Unregister a student from an activity |
| POST | `/auth/login` | Teacher authentication |
| GET | `/auth/check-session` | Validate teacher session |

## Development Guide

For detailed setup and development instructions, including how to set up the MongoDB database and run the application locally, please refer to our [Development Guide](../docs/how-to-develop.md).
