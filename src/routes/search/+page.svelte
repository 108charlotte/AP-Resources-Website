<script lang="ts">
    import Resource from '$lib/Resource.svelte';
    
    const resources = [
        {title: "Heimler's History (Youtube Channel): AP World History Modern", is_paid: "Free", description: "A video tutorial series for students guided by the official course description published by college board. Useful for unit test studying throughout the year, but unit overview videos may oversimplify for those assessments.", link: "https://www.youtube.com/@heimlershistory/featured", rating: 7},
        {title: "Heimler Ultimate Review Guide: AP World History Modern", is_paid: "Paid", description: "A collection of unit review videos and multiple choice questions not found on the main youtube channel. Useful for short, targeted prep for unit assessments, but should be supplimentary if in a challenging class. Does include practice exams with more MCQs (and FRQs, but for FRQs the official ones are by far the best), but not my top pick.", link: "https://heimlershistory.com/", rating: 6}, 
        {title: "Past Exams", is_paid: "Free!", description: "Official questions and grading rubrics from past AP exams. The only drawback is that MCQs are not posted!", link: "https://apcentral.collegeboard.org/courses/past-exam-questions", rating: 10}, 
        {title: "Princeton Review: AP World History", is_paid:"Paid", description: "A comprehensive review book, but may over-fixate on European history and specific details which are not very important or likely to impact your score on the final exam, or even in your class even if you have a difficult teacher. However, practice tests and questions are VERY HIGH QUALITY--I would personally recommend these to suppliment the official exams while practicing throughout the year (so that you are less likely to run out of good questions).", link: "https://www.amazon.com/Princeton-Review-World-History-Preparation/dp/0593517334/ref=pd_lpo_d_sccl_2/135-4087901-6753445?pd_rd_w=SqvPL&content-id=amzn1.sym.4c8c52db-06f8-4e42-8e56-912796f2ea6c&pf_rd_p=4c8c52db-06f8-4e42-8e56-912796f2ea6c&pf_rd_r=AX7EBHCWPBZGKB7A2J9X&pd_rd_wg=fU7hh&pd_rd_r=feccc7ae-a11a-4d06-9124-c3a53669de23&pd_rd_i=0593517334&psc=1", rating: 9}, 
        {title: "UWorld AP World History Practice Q Bank", is_paid: "Paid", description: "A massive supplimentary question bank for AP World history. I found that these questions were very similar to the ones on the actual AP exam and I wish that I had found them sooner!", link: "https://collegeprep.uworld.com/ap-world-history-modern/practice-tests-and-questions/", rating: 7}, 
        {title: "McGraw Hill AP World History Modern", is_paid: "Paid", description: "A physical review book which also comes with a digital platform. I didn't use this one much so I don't have too much to say, but when I did use it I noticed that it had a lot of content that was outdated/from previous exams, and the questions weren't of the highest quality.", link: "https://www.amazon.com/Steps-World-History-Modern-Student/dp/1265317429/ref=sr_1_4?crid=37NYR3U5ABGYT&dib=eyJ2IjoiMSJ9.VRFBifHTdoy6xIV_50G7UueZ1sklNBnuRTLP-ZGeEhY36f85mnI6L6mK7fCadcB45ysH8hVjMVUIbh9Bif8ee4kLAj6tyOv_SQn7HjktlHFZLVX37OsJHlLlrgzm1YHdg3ovgDJI6H6danQK9w3Nj97XPyUFiG0XeLuGz5OdgGUhAQNrKlhfztkyLR3ktfL5whtug3jM_3CTrNuixO4qzhYkHWpx-GgYY4PCtrDV_6U.MhOLqmewjH_FdtMRQIwwTs0Cm7puygMk80jC_mu_hLY&dib_tag=se&keywords=mcgraw+hill+ap+world+history+modern&qid=1753211184&s=books&sprefix=mcgraw+hill+ap+world+history+moder%2Cstripbooks%2C85&sr=1-4", rating: 3}
    ];
</script>

<h1>All Resources</h1>

<div class="grid grid-cols-2 gap-4">
    {#each resources as resource}
        <Resource 
            title={resource.title} 
            description={resource.description}
            link={resource.link}
            is_paid={resource.is_paid}
            rating={resource.rating}
        />
    {/each}
</div>