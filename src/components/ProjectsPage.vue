<template>
    <div id="projects" class="clsProjects">
        <div class="clsContent">
            <div class="clsTitle">Projects</div>
            <div class="clsDescription">I have worked on a wide range of projects, From web apps. Here are some of my projects.</div>
            <div class="clsDescription-content">
                <div class="clsCard" @click="isOpen = true">
                    <img src="../assets/Images/Flight.png" class="clslogo">
                    <div class="cslTechnology">
                        <span>.Net MVC</span>
                        <span>SQL Server</span>
                        <span>Web API</span>
                        <span>jQuery</span>
                        <span>Javascript</span>
                        <span>Bootstrap</span>
                        <span>CSS</span>
                        <span>HTML</span>
                        <span>TFS</span>
                    </div>
                    <div class="clsDec-content">
                        <div class="clsTitle">Online Air Booking Tool</div>
                        <div class="clsDuration">May 2021 - Feb 2023</div>
                        <div class="clsDec">This project unfolds as a revolutionary online ticket selling platform with a broad spectrum of travel services for both consumers and businesses. Operating out of Dubai and Egypt, the platform offers a unified solution for Air tickets, Bus tickets, Hotel reservations, Visa services, and Insurance options. Through seamless integration with local airlines, GDS, and other suppliers, the platform ensures a vast array of options for travelers. The B2C functionality allows individual consumers to explore and purchase various travel services, while the B2B aspect simplifies the process for agents. The unique feature of a single Top-up account streamlines the ticket procurement process for agents, enabling them to efficiently manage and purchase tickets across all available services. This project reflects a commitment to providing a user-friendly, comprehensive, and integrated solution in the travel industry for the Dubai and Egypt markets.</div>
                    </div>
                    <div class="cslFooter"></div>
                </div>

                <div class="clsCard" @click="isOpen1 = true">
                    <img src="../assets/Images/SDK.jpg" class="clslogo">
                    <div class="cslTechnology">
                        <span>.Net Core </span>
                        <span>SQL Server</span>
                        <span>WCF</span>
                        <span>TFS</span>
                    </div>
                    <div class="clsDec-content">
                        <div class="clsTitle">Payment Gateway and SDK Development</div>
                        <div class="clsDuration">Jan 2023 - Feb 2023</div>
                        <div class="clsDec">Collaborated closely with the payment gateway team and mobile network operators to implement the secure and seamless SDK payment flow. Integrate with many banks, UPI and multiple payment gateway like Razorpay. for top up and all airline, Hotel, bus, car Booking.</div>
                    </div>
                    <div class="cslFooter"></div>
                </div>

                <div class="clsCard" @click="isOpen2 = true">
                    <img src="../assets/Images/Synergita.jpeg" class="clslogo">
                    <div class="cslTechnology">
                        <span>.Net Core</span>
                        <span>SQL Server</span>
                        <span>Web API</span>
                        <span>jQuery</span>
                        <span>Javascript</span>
                        <span>Bootstrap</span>
                        <span>CSS</span>
                        <span>HTML</span>
                        <span>SVN</span>
                    </div>
                    <div class="clsDec-content">
                        <div class="clsTitle">Synergita - OKR</div>
                        <div class="clsDuration">Mar 2023 - Dec 2023</div>
                        <div class="clsDec">Synergita's OKR functionality provides a streamlined approach to goal setting and performance management, empowering organizations to define clear objectives and measurable key results that align with their strategic priorities. By facilitating real-time tracking, continuous feedback, and integration with existing performance management processes, Synergita fosters a culture of accountability, transparency, and alignment, enabling teams and individuals to drive meaningful progress and achieve their objectives effectively.</div>
                    </div>
                    <div class="cslFooter"></div>
                </div>

                <div class="clsCard" @click="isOpen3 = true">
                    <img src="../assets/Images/Aspire_System_Logo.jpeg" class="clslogo">
                    <div class="cslTechnology">
                        <span>Vue Js</span>
                        <span>SQL Server</span>
                        <span>Web API</span>
                        <span>Bootstrap</span>
                        <span>CSS</span>
                        <span>SVN</span>
                    </div>
                    <div class="clsDec-content">
                        <div class="clsTitle">Performance Management Roadmap System</div>
                        <div class="clsDuration">Dec 2023 - Feb 2024</div>
                        <div class="clsDec">The Performance Management Roadmap System is a comprehensive framework designed to guide organizations in developing and refining their performance management processes. By providing structured guidance and best practices, it helps companies establish clear goals, align employee objectives with organizational priorities, implement effective feedback mechanisms, and continuously improve performance evaluation and development practices. This system enables organizations to cultivate a culture of accountability, transparency, and growth, ultimately driving enhanced employee engagement and organizational success.</div>
                    </div>
                    <div class="cslFooter"></div>
                </div>

                <div class="clsCard" @click="isOpen4 = true">
                    <img src="../assets/Images/Aspire_System_Logo.jpeg" class="clslogo">
                    <div class="cslTechnology">
                        <span>.Net MVC</span>
                        <span>SQL Server</span>
                        <span>Web API</span>
                        <span>jQuery</span>
                        <span>Javascript</span>
                        <span>Bootstrap</span>
                        <span>CSS</span>
                        <span>HTML</span>
                        <span>SVN</span>
                    </div>
                    <div class="clsDec-content">
                        <div class="clsTitle">High Performance Tracking  System</div>
                        <div class="clsDuration">Mar 2024 - Till</div>
                        <div class="clsDec">The High Performance Tracking System is a dynamic learning tool that facilitates the assignment and tracking of subjects and new programming languages within an educational or professional setting. Through its intuitive interface, users can assign learning objectives, track progress, and assess proficiency levels, enabling individuals and organizations to effectively monitor skill development and knowledge acquisition. With features such as personalized learning paths and performance analytics, the system empowers learners to maximize their potential and achieve high performance in their chosen areas of study.</div>
                    </div>
                    <div class="cslFooter"></div>
                </div>
            </div>
        </div>
    </div>

    <transition name="modal">  
      <div v-if="isOpen">
        <div class="overlay" @click.self="isOpen = false;">
            <div tabindex="-1" class="modal clsPopup">
                <div class="clsPopup-content">
                    <svg v-on:click="isOpen = false" class="clsCancel" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="CloseRoundedIcon" style="position: absolute; top: 10px; right: 20px; cursor: pointer;"><path d="M18.3 5.71a.9959.9959 0 0 0-1.41 0L12 10.59 7.11 5.7a.9959.9959 0 0 0-1.41 0c-.39.39-.39 1.02 0 1.41L10.59 12 5.7 16.89c-.39.39-.39 1.02 0 1.41.39.39 1.02.39 1.41 0L12 13.41l4.89 4.89c.39.39 1.02.39 1.41 0 .39-.39.39-1.02 0-1.41L13.41 12l4.89-4.89c.38-.38.38-1.02 0-1.4z"></path></svg>
                    <div class="clsTitle-1">Online Air Booking Tool - B2C, B2B and BOA</div>
                    <div class="clsTitle-2">May 2021 - Feb 2023</div>
                    <div class="clsSkill">
                        <div>.Net MVC</div>
                        <div>SQL Server</div>
                        <div>Web API</div>
                        <div>jQuery</div>
                        <div>Javascript</div>
                        <div>Bootstrap</div>
                        <div>CSS</div>
                        <div>HTML</div>
                        <div>TFS</div>
                    </div>
                    <div class="clsRole">Full Stack Developer</div>
                    <label>Project Overview</label>
                    <div class="clsProject-dec">Embarked on the development of a comprehensive online ticket selling platform catering to the travel industry in Dubai and Egypt. This versatile platform seamlessly integrates local airlines, Global Distribution Systems (GDS), and various suppliers into a unified system. With a focus on Air tickets, Bus tickets, Hotel bookings, Visa services, and Insurance options, the platform is designed to serve both individual consumers (B2C) and businesses (B2B). The innovative feature of a single Top-up account simplifies the purchasing process for agents, allowing them to procure tickets across all available services with ease.</div>
                    <label>Description</label>
                    <div class="clsdec">This project unfolds as a revolutionary online ticket selling platform with a broad spectrum of travel services for both consumers and businesses. Operating out of Dubai and Egypt, the platform offers a unified solution for Air tickets, Bus tickets, Hotel reservations, Visa services, and Insurance options. Through seamless integration with local airlines, GDS, and other suppliers, the platform ensures a vast array of options for travelers. The B2C functionality allows individual consumers to explore and purchase various travel services, while the B2B aspect simplifies the process for agents. The unique feature of a single Top-up account streamlines the ticket procurement process for agents, enabling them to efficiently manage and purchase tickets across all available services. This project reflects a commitment to providing a user-friendly, comprehensive, and integrated solution in the travel industry for the Dubai and Egypt markets.</div>
                    <!-- <div class="clsButton">
                        <a href="https://roundtrip.in/" target="new">View Live App</a>
                    </div> -->
                </div>
            </div>
        </div>
      </div>
    </transition>

    <transition name="modal">  
      <div v-if="isOpen1">
        <div class="overlay" @click.self="isOpen1 = false;">
            <div tabindex="-1" class="modal clsPopup">
                <div class="clsPopup-content">
                    <svg v-on:click="isOpen1 = false" class="clsCancel" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="CloseRoundedIcon" style="position: absolute; top: 10px; right: 20px; cursor: pointer;"><path d="M18.3 5.71a.9959.9959 0 0 0-1.41 0L12 10.59 7.11 5.7a.9959.9959 0 0 0-1.41 0c-.39.39-.39 1.02 0 1.41L10.59 12 5.7 16.89c-.39.39-.39 1.02 0 1.41.39.39 1.02.39 1.41 0L12 13.41l4.89 4.89c.39.39 1.02.39 1.41 0 .39-.39.39-1.02 0-1.41L13.41 12l4.89-4.89c.38-.38.38-1.02 0-1.4z"></path></svg>
                    <div class="clsTitle-1">Payment Gateway and SDK Development</div>
                    <div class="clsTitle-2">Jan 2023 - Feb 2023</div>
                    <div class="clsSkill">
                        <div>.Net Core </div>
                        <div>SQL Server</div>
                        <div>WCF</div>
                        <div>TFS</div>
                    </div>
                    <div class="clsRole">Full Stack Developer</div>
                    <label>Project Overview</label>
                    <div class="clsProject-dec">The Payment Gateway and SDK Development project involves close collaboration with payment gateway teams and mobile network operators to create a secure and seamless SDK payment flow. The project aims to integrate with multiple banks, UPI (Unified Payments Interface), and various payment gateways such as Razorpay to facilitate top-ups and transactions for airline, hotel, bus, and car bookings. Key objectives include ensuring the security and reliability of payment processing, optimizing the user experience for swift transactions, and enabling seamless integration with booking platforms to enhance customer convenience and satisfaction. Through meticulous development and testing, the project seeks to deliver a robust payment solution that meets the needs of both businesses and end-users, fostering trust and efficiency in online transactions.</div>
                    <label>Description</label>
                    <div class="clsdec">Collaborated closely with the payment gateway team and mobile network operators to implement the secure and seamless SDK payment flow. Integrate with many banks, UPI and multiple payment gateway like Razorpay. for top up and all airline, Hotel, bus, car Booking.</div>
                    <!-- <div class="clsButton">
                        <a href="https://roundtrip.in/" target="new">View Live App</a>
                    </div> -->
                </div>
            </div>
        </div>
      </div>
    </transition>

    <transition name="modal">  
      <div v-if="isOpen2">
        <div class="overlay" @click.self="isOpen2 = false;">
            <div tabindex="-1" class="modal clsPopup">
                <div class="clsPopup-content">
                    <svg v-on:click="isOpen2 = false" class="clsCancel" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="CloseRoundedIcon" style="position: absolute; top: 10px; right: 20px; cursor: pointer;"><path d="M18.3 5.71a.9959.9959 0 0 0-1.41 0L12 10.59 7.11 5.7a.9959.9959 0 0 0-1.41 0c-.39.39-.39 1.02 0 1.41L10.59 12 5.7 16.89c-.39.39-.39 1.02 0 1.41.39.39 1.02.39 1.41 0L12 13.41l4.89 4.89c.39.39 1.02.39 1.41 0 .39-.39.39-1.02 0-1.41L13.41 12l4.89-4.89c.38-.38.38-1.02 0-1.4z"></path></svg>
                    <div class="clsTitle-1">Synergita - OKR</div>
                    <div class="clsTitle-2">Mar 2023 - Nov 2023</div>
                    <div class="clsSkill">
                        <div>.Net Core</div>
                        <div>SQL Server</div>
                        <div>Web API</div>
                        <div>jQuery</div>
                        <div>Javascript</div>
                        <div>Bootstrap</div>
                        <div>CSS</div>
                        <div>HTML</div>
                        <div>TFS</div>
                    </div>
                    <div class="clsRole">Full Stack Developer</div>
                    <label>Project Overview</label>
                    <div class="clsProject-dec">Synergita's OKR project offers a comprehensive platform for organizations to implement and manage Objectives and Key Results (OKRs) effectively. It enables users to set clear and ambitious objectives, define measurable key results, and align them across different levels of the organization. With real-time progress tracking, continuous feedback mechanisms, and integration with performance management processes, Synergita facilitates a culture of accountability, focus, and continuous improvement, empowering organizations to achieve their strategic goals efficiently.</div>
                    <label>Description</label>
                    <div class="clsdec">Synergita's OKR functionality provides a streamlined approach to goal setting and performance management, empowering organizations to define clear objectives and measurable key results that align with their strategic priorities. By facilitating real-time tracking, continuous feedback, and integration with existing performance management processes, Synergita fosters a culture of accountability, transparency, and alignment, enabling teams and individuals to drive meaningful progress and achieve their objectives effectively.</div>
                    <!-- <div class="clsButton">
                        <a href="https://roundtrip.in/" target="new">View Live App</a>
                    </div> -->
                </div>
            </div>
        </div>
      </div>
    </transition>

    <transition name="modal">  
      <div v-if="isOpen3">
        <div class="overlay" @click.self="isOpen3 = false;">
            <div tabindex="-1" class="modal clsPopup">
                <div class="clsPopup-content">
                    <svg v-on:click="isOpen3 = false" class="clsCancel" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="CloseRoundedIcon" style="position: absolute; top: 10px; right: 20px; cursor: pointer;"><path d="M18.3 5.71a.9959.9959 0 0 0-1.41 0L12 10.59 7.11 5.7a.9959.9959 0 0 0-1.41 0c-.39.39-.39 1.02 0 1.41L10.59 12 5.7 16.89c-.39.39-.39 1.02 0 1.41.39.39 1.02.39 1.41 0L12 13.41l4.89 4.89c.39.39 1.02.39 1.41 0 .39-.39.39-1.02 0-1.41L13.41 12l4.89-4.89c.38-.38.38-1.02 0-1.4z"></path></svg>
                    <div class="clsTitle-1">Performance Management Roadmap System</div>
                    <div class="clsTitle-2">Dec 2023 - Feb 2024</div>
                    <div class="clsSkill">
                        <div>Vue Js</div>
                        <div>SQL Server</div>
                        <div>Web API</div>
                        <div>Bootstrap</div>
                        <div>CSS</div>
                        <div>SVN</div>
                    </div>
                    <div class="clsRole">Full Stack Developer</div>
                    <label>Project Overview</label>
                    <div class="clsProject-dec">The Performance Management Roadmap System project is aimed at creating a structured framework to enhance performance management practices within an organization. It involves the development of guidelines, tools, and resources to support various stages of the performance management process, including goal setting, feedback mechanisms, performance evaluation, and employee development. The project seeks to align individual objectives with organizational goals, foster a culture of continuous feedback and improvement, and ultimately drive employee engagement and organizational success. Through a systematic approach, the Performance Management Roadmap System aims to optimize performance management practices to meet the evolving needs of the organization and its employees.</div>
                    <label>Description</label>
                    <div class="clsdec">The Performance Management Roadmap System is a comprehensive framework designed to guide organizations in developing and refining their performance management processes. By providing structured guidance and best practices, it helps companies establish clear goals, align employee objectives with organizational priorities, implement effective feedback mechanisms, and continuously improve performance evaluation and development practices. This system enables organizations to cultivate a culture of accountability, transparency, and growth, ultimately driving enhanced employee engagement and organizational success.</div>
                    <!-- <div class="clsButton">
                        <a href="https://roundtrip.in/" target="new">View Live App</a>
                    </div> -->
                </div>
            </div>
        </div>
      </div>
    </transition>

    <transition name="modal">  
      <div v-if="isOpen4">
        <div class="overlay" @click.self="isOpen4 = false;">
            <div tabindex="-1" class="modal clsPopup">
                <div class="clsPopup-content">
                    <svg v-on:click="isOpen4 = false" class="clsCancel" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="CloseRoundedIcon" style="position: absolute; top: 10px; right: 20px; cursor: pointer;"><path d="M18.3 5.71a.9959.9959 0 0 0-1.41 0L12 10.59 7.11 5.7a.9959.9959 0 0 0-1.41 0c-.39.39-.39 1.02 0 1.41L10.59 12 5.7 16.89c-.39.39-.39 1.02 0 1.41.39.39 1.02.39 1.41 0L12 13.41l4.89 4.89c.39.39 1.02.39 1.41 0 .39-.39.39-1.02 0-1.41L13.41 12l4.89-4.89c.38-.38.38-1.02 0-1.4z"></path></svg>
                    <div class="clsTitle-1">High Performance Tracking  System</div>
                    <div class="clsTitle-2">Mar 2024 - Till</div>
                    <div class="clsSkill">
                        <div>.Net Core</div>
                        <div>SQL Server</div>
                        <div>Web API</div>
                        <div>jQuery</div>
                        <div>Javascript</div>
                        <div>Bootstrap</div>
                        <div>CSS</div>
                        <div>HTML</div>
                        <div>SVN</div>
                    </div>
                    <div class="clsRole">Full Stack Developer</div>
                    <label>Project Overview</label>
                    <div class="clsProject-dec">The project overview for the High Performance Tracking System entails the development of a comprehensive learning tool aimed at enhancing skill acquisition and proficiency tracking in subjects and programming languages. By providing a user-friendly interface and robust functionality, the system enables efficient assignment of learning objectives, progress monitoring, and proficiency assessment. Key features include personalized learning paths, real-time progress tracking, and performance analytics, empowering learners to achieve high levels of proficiency and mastery in their chosen areas of study. Through continuous iteration and improvement, the project aims to meet the evolving needs of learners and organizations, fostering a culture of continuous learning and high performance.</div>
                    <label>Description</label>
                    <div class="clsdec">The High Performance Tracking System is a dynamic learning tool that facilitates the assignment and tracking of subjects and new programming languages within an educational or professional setting. Through its intuitive interface, users can assign learning objectives, track progress, and assess proficiency levels, enabling individuals and organizations to effectively monitor skill development and knowledge acquisition. With features such as personalized learning paths and performance analytics, the system empowers learners to maximize their potential and achieve high performance in their chosen areas of study.</div>
                    <!-- <div class="clsButton">
                        <a href="https://roundtrip.in/" target="new">View Live App</a>
                    </div> -->
                </div>
            </div>
        </div>
      </div>
    </transition>
</template>


<script>
export default {
  data: function() {
    return {
      isOpen: false,
      isOpen1: false,
      isOpen2: false,
      isOpen3: false,
      isOpen4: false
    };
  }
};
</script>