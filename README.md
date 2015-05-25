# How it works
    
    GET /
      check if a teamspeak droplet is present.
      If a droplet is present
        `.touch` it
      Otherwise
         create one
    
    Scheduler
      check if droplet is present.
      If a droplet is present and `updated_at` < 1.hour.ago
        destroy it
