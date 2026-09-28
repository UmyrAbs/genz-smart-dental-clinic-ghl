# GenZ Smart Dental Clinic

## Project Overview

This project is a complete GoHighLevel CRM and automation system built for GenZ Smart Dental Clinic.

The system manages the patient journey from initial lead capture through appointment booking, appointment outcomes, follow ups, and treatment conversion.

## Project Objective

The main objective was to create a structured lead management and automation system that reduces manual follow up and keeps the patient journey organized from lead generation to treatment.

## Patient Journey

Lead Capture → Lead Routing → Appointment Booking → Appointment Outcome → Treatment Conversion → Treatment Started

## Lead Sources

The system handles leads from:

• Dental consultation funnel

• Facebook lead form

Each lead source is tracked in the CRM using the Lead Source custom field.

## CRM Pipeline

The Lead Management pipeline contains these stages:

• New Lead

• Contacted

• Qualified

• Appointment Booked

• Treatment Started

The pipeline provides a clear view of each lead's current position in the patient journey.

## Automation Workflows

### 1. Lead Intake and Routing

Handles leads submitted through the dental consultation funnel.

Main functions:

• Sets Lead Source to Funnel

• Creates a CRM opportunity

• Assigns the lead to the sales user

• Sends an internal notification

• Sends appointment booking email

• Performs follow-up communication

### 2. Facebook Lead Intake

Handles leads submitted through the Facebook lead form.

Main functions:

• Sets Lead Source to Facebook

• Creates a CRM opportunity

• Assigns the lead to the sales user

• Sends an internal notification

• Sends follow-up communication

### 3. Appointment Booked

Triggered when a patient books a Dental Consultation appointment.

Main functions:

• Removes the patient from active lead intake workflows

• Sends appointment confirmation email

• Sends a 24-hour reminder

• Sends a 1-hour reminder

### 4. Appointment Completed

Triggered when the patient attends the appointment.

Main functions:

• Updates the opportunity stage to Qualified

• Notifies the assigned sales user

• Sends post-consultation follow-up email

### 5. Appointment No Show

Triggered when a patient does not attend the appointment.

Main functions:

• Notifies the assigned sales user

• Sends follow-up email

• Sends final follow-up email

### 6. Appointment Cancelled

Triggered when a patient cancels the appointment.

Main functions:

• Notifies the assigned sales user

• Sends rescheduling email

• Sends final rescheduling follow-up email

### 7. Treatment Conversion

Triggered when an opportunity is moved to Won.

Main functions:

• Notifies the assigned sales user

• Sends treatment confirmation email

• Checks whether treatment has started

• Sends follow-up communication when treatment has not started

• Ends the workflow after the final follow-up

## Email System

Email sending was configured using the custom domain:

hello@genzsmart.cyou

Email authentication was configured with:

• SPF

• DKIM

• DMARC

The sending domain and email analytics were also verified during testing.

## Facebook Integration

Facebook lead generation was connected with GoHighLevel.

The Facebook lead form was mapped to CRM contact fields, including:

• Full Name

• Email

• Phone Number

• Dental inquiry information

Test lead synchronization was performed to verify the Facebook to CRM connection.

## Funnel

The project includes a Dental Consultation funnel containing:

• Landing page

• Lead form

• Thank You page

• Dental Consultation calendar

The funnel provides the entry point for new dental consultation leads.

## Testing and Verification

The system was tested through the main lead and appointment scenarios.

Testing included:

• Funnel lead submission

• Facebook lead submission

• CRM contact creation

• Lead source tracking

• Opportunity creation

• Sales user assignment

• Appointment booking

• Appointment confirmation

• Appointment completion

• Appointment no-show

• Appointment cancellation

• Treatment conversion

• Email delivery

## Technology

• GoHighLevel

• CRM

• Workflow Automation

• Funnel Builder

• Calendar

• Email Automation

• Facebook Lead Integration

## Project Documentation

Project screenshots are available in the `Screenshots` folder.

The screenshots document the funnel, booking calendar, CRM pipeline, automation workflows, and email system.
