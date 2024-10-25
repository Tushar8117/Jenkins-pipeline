# FROM python:3
# RUN pip install django==3.2

# COPY . .

# RUN python manage.py migrate
# EXPOSE 8000
# CMD ["python","manage.py","runserver","0.0.0.0:8000"]


FROM python:3.12

# Install Django and setuptools
RUN pip install django==3.2 setuptools

# Copy project files
COPY . .

# Run migrations
RUN python manage.py migrate

# Expose the application port
EXPOSE 8000

# Command to start Django server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

