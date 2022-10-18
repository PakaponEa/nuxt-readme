targetคุณสามารถรันคำสั่งเหล่านี้ได้ทั้งนี้ขึ้นอยู่กับ

	server server-side and on the clint-side
		nuxt dev: เริ่มเซิร์ฟเวอร์การพัฒนา
		nuxt build: รวมแอปพลิเคชัน Nuxt ของคุณสำหรับการผลิต    **แก้ไขต้อง build ใหม่   server-side and on the clint-side
		nuxt start: เริ่มเซิร์ฟเวอร์ที่ใช้งานจริง
	static  :wanted to load this up on an s3 bucket or github pages
		nuxt dev: เริ่มเซิร์ฟเวอร์การพัฒนา (รับรู้แบบคงที่)
		nuxt generate: รวมแอปพลิเคชัน Nuxt ของคุณสำหรับการผลิตหากจำเป็น (การรับรู้แบบคงที่) และส่งออกแอปพลิเคชันของคุณเป็น HTML แบบคงที่ในdist/ไดเร็กทอรี  
		nuxt start: ให้บริการแอปพลิเคชันการผลิตของคุณจากdist/
		
	
	เพื่อปรับปรุงประสบการณ์ผู้ใช้และบอก Nuxt ว่าคุณต้องการส่งออกแอปพลิเคชันของคุณไปยังโฮสติ้งแบบคงที่ เราขอแนะนำtargetตัวเลือกในnuxt.config.js:	
	nuxt generatewith target: 'static'
	
	npm run preview ต้อง generate ก่อนและตั้งค่า nuxt generatewith target: 'static'
	
	
	
	
	
	- cd /dir
	
	npm install nuxt
	
	
	
	ต้องไปแก้ folder G:\Dek-D\demo\package\public\images\users ก่อนและค่อยบิ้ว หลังจากนั้น start ถึงจะเปลียนรูป
	
	มีทำการ generate จะสร้าง folder G:\Dek-D\demo\package\dist ขึ้นมาสามารถเข้าไปแก้ข้อมูล
	
	
	- [1] static    ***หลัง generate เข้าไปเปลี่ยนรูปใน folder G:\Dek-D\demo\package\dist\images\users หน้าเว็บก็เปลี่ยนรูปไปตามรูปที่เปลี่ยน
	nuxt generate:
	G:\Dek-D\demo\package>npm start

		> start
		> nuxt start

		Nuxt CLI v3.0.0-rc.5                                                                                          11:01:20
		i Node.js version: 16.17.1                                                                                    11:01:21
		i Preset: nitro-prerender                                                                                     11:01:21
		i Working dir: .output                                                                                        11:01:21
		i Starting preview command: npx serve -s ./public                                                             11:01:21
																													  11:01:21
		INFO: Accepting connections at http://localhost:3000.
		
		
		ต้องไปแก้ folder G:\Dek-D\demo\package\public\images\users ก่อนและค่อยบิ้ว หลังจากนั้น start ถึงจะเปลียนรูป
		มีทำการ build จะสร้าง folder G:\Dek-D\demo\package\dist ขึ้นมาไม่สามารถเข้าไปแก้ข้อมูล
		
	- [2] server
	nuxt build:
	G:\Dek-D\demo\package>npm run start

		> start
		> nuxt start

		Nuxt CLI v3.0.0-rc.5                                                                                          11:05:01
		i Node.js version: 16.17.1                                                                                    11:05:01
		i Preset: node-server                                                                                         11:05:01
		i Working dir: .output                                                                                        11:05:01
		i Starting preview command: node ./server/index.mjs                                                           11:05:01
																													  11:05:01
		Listening on http://0.0.0.0:3000/
		
		
	*** Deply GitHub Pages
		https://www.youtube.com/watch?v=lG9y6WKcyeE
		https://devahoy.com/tutorials/nuxtjs-fundamental/nuxt-deployment
		https://app.netlify.com/teams/pakaponea/overview
		
		
	*** 
	G:\Dek-D\demo\package\dist\_nuxt\entry.57eac197.css = ไฟล์ css ทั้งหมด
	
	***
	https://nuxtjs.org/deployments/github-pages/
	
	***
	Two Irresistible Ways To Deploy Your Nuxt.js Application (Universal and Static)
	server server-side and on the clint-side
	https://www.youtube.com/watch?v=vlUZw1J0kwM