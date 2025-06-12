# PostgreSQL_Assignment


 1. What is PostgreSQL?

    PostgreSQL একটি ওপেন সোর্স রিলেশনাল ডাটাবেজ ম্যানেজমেন্ট সিস্টেম (RDBMS) যা ডেটা সংরক্ষণ, পরিচালনা ও বিশ্লেষণের জন্য ব্যবহৃত হয়। এটি ACID কমপ্লায়েন্ট এবং জটিল কোয়েরি, ট্রানজেকশন ও এক্সটেনশন সমর্থন করে।


 2. What is the purpose of a database schema in PostgreSQL?

    একটি ডাটাবেজ স্কিমা হলো ডাটাবেজের মধ্যে লজিক্যাল স্ট্রাকচার যা টেবিল, ভিউ, ফাংশন ইত্যাদি সংগঠিত করে। এটি মাল্টি-ইউজার এনভায়রনমেন্টে তথ্য পৃথক করে রাখতে সাহায্য করে এবং নিরাপত্তা ও মেইনটেনেন্স সহজ করে তোলে।


 3. Explain the Primary Key and Foreign Key concepts in PostgreSQL.

    - Primary Key এমন একটি কলাম যা টেবিলের প্রতিটি রেকর্ডকে ইউনিকভাবে শনাক্ত করে। এটি NULL হতে পারে না।

    - Foreign Key এমন একটি কলাম যা অন্য টেবিলের প্রাইমারি কী এর সাথে সম্পর্ক তৈরি করে, যার মাধ্যমে দুটি টেবিলের মধ্যে রিলেশন তৈরি হয়।



 5. Explain the purpose of the WHERE clause in a SELECT statement.

    WHERE ক্লজটি SELECT, UPDATE অথবা DELETE কোয়েরিতে নির্দিষ্ট শর্ত দিয়ে ফলাফল ফিল্টার করতে ব্যবহৃত হয়। এটি নির্দিষ্ট রো বা তথ্য নির্বাচন করতে সাহায্য করে।
    
    -উদাহরণ:

        SELECT * FROM species WHERE conservation_status = 'Endangered';




 7. How can you modify data using UPDATE statements?

    UPDATE স্টেটমেন্ট ব্যবহার করে বিদ্যমান ডেটা পরিবর্তন করা যায়। এতে SET দিয়ে নতুন মান নির্ধারণ করা হয় এবং WHERE ক্লজ দিয়ে নির্দিষ্ট রেকর্ড বেছে নেওয়া হয়।

    -উদাহরণ:

        UPDATE species
        SET conservation_status = 'Historic'
        WHERE discovery_date < '1800-01-01';
