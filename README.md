# BoCo-Signups

Project Topic:

This is a project I am working on in my spare time for Bouquet Collective (BoCo), a non-profit based in Santa Barbara that brings joy into people's lives using flowers that were “destined for the dumpster.” Growers across Santa Barbara County donate flowers that are still beautiful but no longer sellable, and BoCo collects them, makes them into bouquets, and delivers them to terminally ill patients, families going through tough times, or anyone in need of some cheer. It runs entirely on volunteers.

BoCo is in its early stages, and Santa Barbara is only the first chapter. Austin and Palo Alto are following soon, and all of the chapters will be using the same tools, so while I am building this for Santa Barbara, it has to be something a new chapter can pick up and use rather than rebuild.

For BoCo to run efficiently, the coordinators need all of their volunteer data stored in one place that is easy to get at. That is the first step of this project. Eventually, it will be paired with a platform where volunteers enter their personal information, sign up, and check in and out, with all of that data going to one location the coordinators can access.

Problem Statement:

Right now, everything to do with personal information, sign-ups, and volunteering is handled manually, and none of it is connected. The coordinators have no way to consolidate what they know about their volunteers, and no single place to look any of it up. A new chapter would be starting from exactly the same position, since there is nothing built to hand them.

Dataset:

At the moment, I have created a fake dataset that models the data we will be collecting once this project is finalized. The entries we will be tracking are:

    volunteer_id 
  
    name_first
  
    name_last

    email
    
    phone
  
    ref_name
  
    event_date
  
    sign_up
  
    time_in
  
    time_out
  

Because this will eventually be real people's contact information, it matters who can see it. The live version will sit behind a login that only coordinators can use, and volunteers will be entering their own information, so they know what is being stored. The names, emails, and phone numbers are there so coordinators can run an event. I have not done any direct analysis, but the data we anticipate collecting will be helpful in the future once BoCo becomes a bigger organization. For now, some simple analysis can be conducted through volunteer_id, which is tied to each volunteer individually. 
  
Data Analysis and anticipated results/usage:

The first thing this gives the coordinators is the ability to pull any information they need about their volunteers. Beyond that, it lets them see trends they cannot see today: which days of the week volunteers turn out for, how often people come back, whether sign-ups tend to turn into no-shows, whether people are arriving late and leaving early, and whether one volunteer is referring a lot of the new ones.

Tools:

  Excel: .csv file of sample data
  
  Python (pandas): data cleaning
  
  SQLite: storage
  
  Tableau: dashboard
  
  Basic numbers, stats, and graphics
  

Future Enhancements:

With enough sign-up and check-in data, this could help coordinators staff an event and make plans for delivering flowers.
The same data could also track what volunteers worked on, how many bouquets were made and delivered, and how many flowers were saved from the dumpster. Those are the numbers that show whether BoCo is growing, and the ones a new chapter would want to track as part of their operation and for fundraising.
